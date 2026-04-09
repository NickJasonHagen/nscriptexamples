## String methods
```swift
mystring = "hello world"
characterlenght = len(split(mystring)) // splits the string to a array by characters and return the lenght
hexstring = stringtohex(mystring) // string to hex
string = hextostring(hexstring)// convert hex to string
firstchar = prefix(string)
lastchar = suffix(string)
first3chars = fromleft(string,3)// returns first 3 chars
last3chars = fromright(string,3) // returns last 3 chars
trimmed = trimleft(string,1) // trims 1 char from the left
trimmed = trimright(string,1) // trims 1 char from the right
encrypted = encrypt(string,"mypassword") // custom encryption
encrypted = decrypt(string,"mypassword") // custom encryption
ensuredstring = string_or(string,"this sets when the string is empty")
base = stringtobase64(string) // base64 encrypted
string = base64tostring(base) // base64 decrypt
formattedstring = string(string,base) // formats all arguments to 1 string
````

