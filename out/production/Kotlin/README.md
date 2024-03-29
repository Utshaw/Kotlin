# Kotlin
- Language Tutorial: [Learn Kotlin in 12 Minutes - 2021](https://youtu.be/iYrgWO2oibY)

## [How Kotlin works in android](https://stackoverflow.com/questions/47153013/how-does-kotlin-code-get-executed-in-an-android-application-and-how-is-it-diffe)

- Kotlin compiler takes Kotlin code and emites JVM byte code in `.class` files
- Android gradle plugin takes the JVM bytecode and converts it into Dalvik bytecode and packes it into .apk
- When the `.apk` file is installed on device ART converts Dalvik bytecode and converts that into machine code
- The machine code is executed

## Variable

- every variable must have a type (statically type)
- `val` : readonly
- `var` : read & write permission
```
val firstname: String = "Rahul"
var weight = 1232

```
## list
- `mutableListOf` - mutable list (can add)
- `listOf` - immutable list (can't add)
```
val names = mutableListOf<String>("Farhan", "Tanvir", "Utshaw")
for(name in names) {
    println(name)
}
```
## for loop
```
for(i in 1..5) {
    println(i)
}
```
## function
```
fun foo(name: String): Int {
    print("Hello $name")
    return 100
}
```