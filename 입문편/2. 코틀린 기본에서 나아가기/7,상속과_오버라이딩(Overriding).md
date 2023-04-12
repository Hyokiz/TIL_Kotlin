# 상속과 오버라이딩(Overriding)

- open으로 method를 자식에게 내려줄 수 있다.
- override로 덮어씌울 수 있다.

```
fun main() {
//    Parents().disease()
    Child().disease()
    Child().doing()
}

open class Parents() {
    fun doing() {
        println("자식을 돌봅니다.")
    }

    open fun disease() {
        println("비염이 있습니다.")
    }
}

class Child() : Parents() {

    override fun disease() {
        super.disease()
    }
}
```

- 다음과 같이 사용 시 부모의 method를 덮어씌울 수 있음

```
fun main() {
//    Parents().disease()
    Child().disease()
    Child().doing()
}

open class Parents() {
    fun doing() {
        println("자식을 돌봅니다.")
    }

    open fun disease() {
        println("비염이 있습니다.")
    }
}

class Child() : Parents() {

    override fun disease() {
//        super.disease()
        println("겁이 많습니다.")
    }

}
```