fun main() {
    println("TDD")
    if (sumaParesTest())println("Passed")else println("Failed")
    if (sumaImparesTest())println("Passed")else println("Failed")
    if (sumaCuandoLosNumsSeanNegativosTest())println("Passed")else println("Failed")


}

fun sumaPares(a:Int,b:Int): Int{
    if (a%2!=0)return -1
    if (b%2!=0)return -1
    if (a < 0 && b < 0)  return -1 
    

    return a+b
}

fun sumaParesTest():Boolean{
    val actualValue= sumaPares(2,2)
    val expectedValue= 4
    return actualValue == expectedValue
}
fun sumaImparesTest():Boolean{
    val actualValue= sumaPares(3,3)
    val expectedValue= -1
    return actualValue == expectedValue
}
fun sumaCuandoLosNumsSeanNegativosTest():Boolean{
    val actualValue= sumaPares(3,3)
    val expectedValue= -1
    return actualValue == expectedValue
}
