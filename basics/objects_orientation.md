# a class in nscript is global , meaning its accesable everywhere
## and only one can exist under a unique name.
```swift

class myclass{
    self.info = "hello im a property of myclass"
}
````

# if we want to spawn a class from myclass under a new name we can use this
```swift
// you can print a property tagging the object from the spawned class name,
// here we use it by the name created by parsing the class scope
print(myclass.info)

newclass : myclass
print(newclass.info)
````
# we can also attache functions to classes which also be included on spawning new classes

```swift
class animal{
   // this is a built in function which automaticly triggers whenever a spawn is created
   func construct(){
        print("animal added:",self)
    }
    // this is a built in function which automaticly triggers whenever a object is deleted
    func destruct(){
        print("animal wiped:",self)
    }
}
//
class dog : animal{
    func walk(){
      print("[",self," walking loudly]","green")// print with more then 1 arg will use the last one for the color the rest is a concatinated string
    }
    self.eats ["treats","dogfood","humanfood"]
}
````

# lets spawn scooby and pluto and let em walk
```swift
scooby : dog
pluto : dog
scooby.walk()
pluto.walk()
````

# mixing classes or side inherent
## when including myclass to scooby who is already a spawn of dog it will overwrite all functions and properties
## from the tagged class.
```swift
scooby : myclass
class kitty{
    func walk(){
      print("[",self," walking loudly]","green")// print with more then 1 arg will use the last one for the color the rest is a concatinated string
    }
    self.eats ["treats","catfood"]
}
// now we set scooby as kitty, which has the same functions and properties as dog, so the dogs implements will be override by kittys
// however scooby still has scooby.info as it remained
scooby : kitty
print(scooby.info)
````

# lets spawn dynamic objects from a loop
```swift
array = ["Jhonno","jack","slinky","poes"]
for xobject in array{
    // by prefixing the variable with a * it will evaluate the variable before using the name.
    // otherwise it would create a object by the name xobject
    *xobject : kitty
}
// deleting objects ( in this case from a loop!)
for xobject in array{
    // this function deletes a object by a reference
    // if the object contains a function .destruct() it will be triggered before deleting it (clean up systems eg).
    object::delete(xobject)// we give it as a variable (argument) which will evaluate it so no * required here
}
````

# function dispatching
```swift
class myclass{
    func myfunc(){
        // some code
    }
}

var = "myclass"
var2 = "myfunc"

// evaluate the classname and/or the function name
*var.*var2()

````
# object index

```swift
listofallproperties = object::index("someobjectname")
listofallfunctions = object::functions("someobjectname")
object::delete("someobjectname") // deletes the entire object
object::deleteproperty("someobjectname","somepropertyname") // deletes the entire object

// nscript objects and simple json | only does properties as string key/stringvalue
somejsonstring = object::tojson("someobjectname") // map a nscript object to a json string
object::fromjson("someobjectname",somejsonstring) // map a nscript object from a json string

````
