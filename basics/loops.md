## Regular loops
these loops prevent coroutines from executing
this is a traditional endless loop which only ends when break is given

example loop which breaks after 2 seconds
```swift
timer = timerinit()
loop{
    if timerdiff(timer) > 1999{
        break
    }
}
````

## for loops
```swift
// for in array iterates thru a vector
array = [1,2,3,4,5]
for i in array{
    print(i)
}
// for to , a counted loop
for i to 10{
    print(i)//prints a number of iteration
}
// begin from a different number then 0
for i=5 to 10{
    print(i)//prints a number of iteration
}
````
