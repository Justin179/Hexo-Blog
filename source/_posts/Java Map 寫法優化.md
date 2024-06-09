---
title: Java Map 寫法優化
date: 2024-06-09
tags:
- Java
- 寫法優化
- Leetcode
category:
- [技術,Java]
hide: false
top: false
---

<mark>改寫前</mark>

這個寫法是為了避免當`map.get(key)`為`null`時，直接`.add()` 發生`NullPointerException`

```java
        Map<String,List<String>> map = new HashMap<>();
        for(String str : strs){
            String key = sortStr(str);
            // key不存在於map 
            if(map.get(key)==null){
                // 手動創建一個新的List 
                List<String> temp = new ArrayList<>();
                temp.add(str);
                // List放回map 
                map.put(key,temp);
            }else{
                // map原本就有該key，就直接取出List 
                List<String> strings = map.get(key);
                strings.add(str);
            }
        }
```



<mark>改寫後</mark>

更好的寫法是，先透過 `map.computeIfAbsent()` 來確保在key不存在於map時，先在map中加進該 key:value pair，就可以避免上面`map.get(key)`為`null`的情況

```java
        Map<String,List<String>> map = new HashMap<>();
        for(String str : strs){
            String key = sortStr(str);
            // 確保在key不存在於map時，先在map中加進該key:value pair 
            map.computeIfAbsent(key,k->new ArrayList<>());
            map.get(key).add(str);
        }
```

