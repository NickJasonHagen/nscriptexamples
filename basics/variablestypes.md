## variable types
```swift
//local scope variables
myvar = "i exist until the block is done"
// usize/int
myvar = 123
//float
myvar = 0.1
myvector = ["string",1,0.923] // vector
anothervector = [
 1,
 2,
 3
]
//global variable
$globalvar = "im accesable from everywhere"
settings.info = "this is property info of object settings"

// dispatching objectnames and properties
myobjectreference = "settings"
myprop = "info"

print(*myobjectreference.info) // this uses myobjectreference as a reference to the actual object name, it will evaluate the variable and use the value as a object
print(*myobjectreference.*myprop) // this uses myobjectreference and myprop as a references to the actual object and property name, it will evaluate the variables and use the values as a object and property references
````

