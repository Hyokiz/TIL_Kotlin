# 함수(Function)란?

- 함수는 기능이다.
- 인자에 타입을 지정해줘야 한다.

```
fun main() {
    abc()
    abc2()
    sum(20, 40)
}

fun abc() {
    val a = 10
    val b = 20
    val c = a + b
    println(c)
}

fun abc2() {
    val a = 20
    val b = 40
    val c = a + b
    println(c)
}

fun sum(a : Int, b : Int) {
    println(a + b)
}
```

- return 할 경우도 타입을 지정해주어야 한다.

```
fun main() {
    println(sum(20, 40))
}

fun sum(a : Int, b : Int) : Int {
    val result = a + b
    return result
}
```
```
fun main() {
    bobMaking(5)
}

fun bobMaking(time: Int) {
    println("$time 분 후에 밥이 완료됩니다.")
}
```
