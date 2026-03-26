# variable types.
```swift
username = "Barry Batsbek" // a string
age = 20 // a int
belly = 0.876 // float
admin = true
time = cat(@hour,":",@min)// concatinates a string formatting the time using built in macros @hour and @min
````

# check for equals
```swift
if username == "Gerret" {
    // do something here
}
````
# if and
## name equals and age bigger or equals
```swift
if username == "Gerret" && age >= 18{
    // do something here
}
````
# name does not equals , age bigger then , or admin is true
```swift
if username != "Gerret" && age > 17 || admin == true{
    // do something here
}
````
# rather use and or ? choice also works !
```swift\
if username != "Gerret" and age > 17 or admin == true{
    // do something here
}
````
# else
```swift
if admin == true{
    // do something here
}
else {
    // do something when not admin
}
````
# else
```swift
if belly > 0.9{
    // energized and content
}
else if belly > 0.6 {
    // wants a snack
}
else if belly > 0.4 {
    // growling
}
else{
    // starving
}
````


