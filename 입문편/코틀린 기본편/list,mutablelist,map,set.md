# list, mutablelist, map, set

## List

```
fun main() {
    /* 전에 만든 방식 */
    /*
    val testList1 = listOf("a", "b", "c")
    println(testList1)
    */
    val testList2 = mutableListOf<String>("a", "b", "c")
    println(testList2)
    testList2.add("d")
    println(testList2)
    testList2.remove("a")
    println(testList2)

    val testList3 = arrayListOf<String>("a", "b", "c")
}
```

## MutableList

- add, remove

```
fun main() {
    /* 전에 만든 방식 */
    /*
    val testList1 = listOf("a", "b", "c")
    println(testList1)
    */
    val testList2 = mutableListOf<String>("a", "b", "c")
    println(testList2)
    testList2.add("d")
    println(testList2)
    testList2.remove("a")
    println(testList2)

    val testList3 = arrayListOf<String>("a", "b", "c")
}
```

## Map

- list의 경우 add 였으나, map의 경우 put

```
fun main() {
    /*
    val mutableList1 = mutableListOf<Int>()
    mutableList1.add(5)
    mutableList1.add(10)
    mutableList1.add(15)
    mutableList1.add(22)

    val mutableList2 = mutableListOf<String>()
    mutableList2.add("유리")
    mutableList2.add("철수")
    mutableList2.add("짱구")
    mutableList2.add("훈이")

    val findIndex = mutableList1.indexOf(10)
    println(findIndex)
    println(mutableList2[findIndex])
    */

    val testMap1 = mutableMapOf<Int, String>()
    testMap1.put(5, "유리")
    testMap1.put(10, "철수")
    testMap1.put(15, "짱구")
    testMap1.put(22, "훈이")

    println(testMap1[15])
}

```

## Set

- 중복값은 들어가지 않음
- add, remove

```
fun main() {
    val testSet1 = mutableSetOf<String>("a", "b", "c")
    testSet1.add("d")
    testSet1.add("e")
    testSet1.add("e")
    println(testSet1)
}

```