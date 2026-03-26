
## simple match scope (faster then if statements)
using a return within this scope will return the previous scope
```swift
match @sec{
    1 =>{
        // some code
        // when second = 1
    }
    2 3 4 => { // checking multiple , 2 3 and 4
        // some code
    }
    _ =>{ // optional if none match
        // otherwise !
    }
}
````
## using a match to set a variable
when catching the match scope to a variable use the return scope, whatever returns will fill the myvar
you can use return *
or by onewordlines variable / macro / number / staticstring / int / float / bool
```swift
myvar = match @hour{
    4 5 6 7 8 9 10 11 =>{
        return "Good morning"
    }
    12 13 14 15 16 17  => { // checking multiple , 2 3 and 4
        return "Good afternoon"
    }
    _ =>{ // optional if none match
        return "Good night"
    }
}
print(myvar) // output the set variable
````
