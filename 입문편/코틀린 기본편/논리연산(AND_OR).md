# 논리연산(AND OR)

```
fun main() {
    val a = "남자"
    val b = 20

    if (a == "남자" && b >= 20) {
        println("AND 만족")
    } else {
        println("AND 불만족")
    }

    val c = "남자"
    val d = 30

    if (c == "남자" || d >= 30) {
        println("OR 만족")
    } else {
        println("OR 불만족")
    }
}
```

```
fun main() {
    val student = mutableMapOf<Int, String>()
    student[99] = "민지"
    student[20] = "철수"
    student[35] = "민수"
    student[48] = "가영"
    student[100] = "하영"
    student[22] = "수진"
    student[45] = "수달"
    student[88] = "캥거루"
    student[91] = "코알라"
    student[87] = "악어"
    student[54] = "코끼리"
    student[42] = "하마"

    // 점수가 50점 이상이고 학생의 이름 길이가 3 이상만 프린트
    for (i in student) {
        if (i.key >= 50 && i.value.length >= 3) {
            println(i.value)
        }
    }
}
```