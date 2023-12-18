---
tags: [Kotlin]
title: Kotlin Notes
created: '2023-12-18T16:22:45.222Z'
modified: '2023-12-18T17:57:32.807Z'
---

# Kotlin Notes
- [Crash course](https://www.youtube.com/watch?v=5flXf8nuq60)

## Basic notes

- Always use ```val``` for values unless you want to make them variables with ```var``` .

- Kotlin is a ```NULL``` safe language unlike Java is so we can use it as a value.
  - To do so, we need to make the variable/valua nullable by adding a ? after the data type.
    ```val x: Int? = null```
  - By default ```readLine()``` returns ```String?``` allowing it to be ```null``` .
  - When converting null-able String to Int, we can use ```!!``` to assume that it's not null. This is not recommended.
    ```val result = num1!!.toInt() + num2!!.toInt()```
  - In that case, better set a default value if the input was null.
    ```val num1 = readLine() ?: "0"```

- For creating lists we can use,
  - Immutable list (can not make changes)
    ```val shopList = listOf<String>('a','b','c')```
    - But we also can ignore the ```<String>``` since Kotlin identifies the data type.
  - Mutable list (editable)
    ```val shopList = mutableListOf('a','b','c')```

- 