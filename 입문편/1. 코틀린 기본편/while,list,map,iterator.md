# While, List, Map, Iterator

## While

```kotlin
fun main() {
    var count = 0
    while (count < 10) {
        println(count)
        count++
    }
}
```

## List

```
fun main() {
    val testList1 = mutableListOf<String>("a", "b", "c")
    println(testList1)
    for (i in testList1) {
        println(i)
    }
}
```

## Map

- Map이 파이썬 dictionary 개념

```
fun main() {
    val testMap1 = mutableMapOf<Int, String>()
    testMap1.put(5, "a")
    testMap1.put(10, "b")
    testMap1.put(15, "c")
    println(testMap1)

    for (i in testMap1) {
        println(i)
    }

    val testMap2 = mutableMapOf<Int, String>()
    testMap2[5] = "A"
    testMap2[10] = "B"
    testMap2[15] = "C"
    println(testMap2)
}

```

## Iterator

- next() : 다음 값 표시
- hasNext() : 다음 값이 있다면 true, 없다면 false

```
fun main() {
    val testList2 = mutableListOf<String>("a", "b", "c")

    val testIterator = testList2.listIterator()

    println(testIterator.next()) // a
    println(testIterator.next()) // b
    println(testIterator.hasNext()) // true
    println(testIterator.next()) // c
    println(testIterator.hasNext()) // false
    println(testIterator.previous()) // c
    println(testIterator.previous()) // b
    println(testIterator.previous()) // a

    while (testIterator.hasNext()) {
        println(testIterator.next())
    }
}
```