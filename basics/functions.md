# functions
## simple function
a simple function example
```swift
// defile a custom function block
func helloworld(){
    print("hello world")
}

helloworld()

````
## function returns
functions can return something back to the spot where its used
```swift
func ping(){
    print("ping")
    return "pong"// is going the be the value which this block returns
}

myvar = print(ping())
myvar !//<-- shows the debug state of this onelinerword


````
## function arguments and returns
functions can also take multiple values from elsewhere and use them to return something new
```swift
func newname(name,sirname){
    fullname = cat(name,sirname)
    splitname = split(fullname,"")// split the name by characters
    splitname = arrayreverse(splitname)
    return join(splitname,"")// reconstruct the reversed array
}

print(newname("Gokkie","keumus")) !


````

