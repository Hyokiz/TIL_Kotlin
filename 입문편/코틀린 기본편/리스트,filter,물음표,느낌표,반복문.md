# 리스트, filter, 물음표, 느낌표, 반복문

## 리스트 만드는법

```
fun main() {
	val testList1 = ArrayList<String>();
    testList1.add("a");
    testList1.add("b");
    testList1.add("c");
    
    println(testList1) // [a, b, c]
    
    val testList2 = listOf("a", "b", "c");
    println(testList2); // [a, b, c]
    
    val testList3 = mutableListOf<String>("a", "b", "c");
    println(testList3)
}
```

## filter

```
fun main() {
	val testList4 = listOf("student1", "student2", "student3", "student4", "teacher1", "student5")
    println(testList4);
    println(testList4.filter { it.startsWith("s") } )
}
```

## 물음표, 느낌표

### 물음표

null일수도 있는 값을 표현

### 느낌표

null이 아니다 라는 것을 표현
느낌표 두개로 표현

```kotlin
fun main () {
    var test1 : String = "a"
    var test2 : String = "b"

    test1 = test2
    println(test1)

    var test3 : String = "c"
    var test4 : String? = "d"

//    test3 = test4 // null 일 수 있는 값을 null이 아닌 값에 집어넣게 되면 안된다.
    test3 = test4!!
    print(test3)
}
```

## 반복문

- in으로 반복 가능.
- .. 으로 그 범위를 표현 가능

```kotlin
fun main () {
    val testList6 = listOf<String>("a", "b", "c", "d", "e", "f")
    for (i in testList6) {
        println(i)
    }

    for (i in 1..10) {
        println(i)
    }
}
```

- $표시로 뒤에 변수 삽입 가능

```
fun main () {
    for (i in 1..10 step 3) {
        println(i)
    }

    for (i in 1..3) {
        println("i의 값은 : $i")
    }
}
```

### 이중 반복문

```
fun main () {
    for (i in 1..3) {
        for (j in 1..3) {
            println("i is $i, j is $j")
        }
    }
}
```

