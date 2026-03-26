```javascript
 fn-id:0 |  printraw(string,color) // returns the given string, colors first char as a string "r" for red, blue,purple yellow green,magenta, for brightcolors add "b" so for red "br" for bright blue "bb"
 fn-id:1 |  cos(number) // cos on number
 fn-id:2 |  sin(number) // sin on number
 fn-id:3 |  add(number,toadd)  // adds the number given by the numberto add
 fn-id:4 |  subtract(number,tosubtract)  // subtracts the number given by the numbertosubtract
 fn-id:5 |  multiply(number,tomultiply)  // multiplies the number given by the numbertomultiply
 fn-id:6 |  devide(number,todevide)  // subtracts the number given by the numbertodevide
 fn-id:7 |  add(number,toadd)  // adds the number given by the numberto add
 fn-id:8 |  is_alphabetic(string)  // Checks if a string is alphabetic, returns a bool
 fn-id:9 |  timerdiff(timerinit)  // takes a timervar created by timerinit() returns the difference in ms
 fn-id:10 |  timerinit()  // returns a timervar, can be used with timerdiff(var) to check difference in time ms
 fn-id:11 |  trim(string)  // returns a trimmed string, this strips spaces in front and at end
 fn-id:12 |  len(vec)  // takes a vector returns the size
 fn-id:13 |  vec(string,a,b,c,..endless)  // can take any ammount of arguments , creates a vector out of each given argument and returns it.
 fn-id:14 |  uppercase(string)  // returns the given string in UPPERcase
 fn-id:15 |  replacebyref(referencevar,find,replace)  // this doesnt return anything, it will replace found string in the var given as referencevar,
 if using multiple lines with replace() this will optimize it by a lot
 fn-id:16 |  lowercase(string)  // returns the given string as lowercase
 fn-id:17 |  stringbetween(string,beginstring,endstring)  // searches a string by a begin and end, returns the first result as a string.
 if none found returns a empty string
 fn-id:18 |  split(string,splitdelimeter)  // splits a string into a vector by a given delimeter.
 to split a string by each character give a empty string as delimeter
 fn-id:19 |  contains(string,containsstring)  // returns a bool if a string contains a substring
 fn-id:20 |  stringtoeval(string)  // replaces all spaces and special characters of a given string
 usecases: to set properties of them, or create identifiers during runtime
 fn-id:21 |  replace(string,find,replace)  // returns a new string if the substring is found it will replace it.
 fn-id:22 |  join(vector,delimeter)  // returns a string of a given vector it will join the items by the delimeter
 fn-id:23 |  instring(string,substring)  // returns a bool if the string contains a substring ( same as contains() )
 fn-id:24 |  fromleft(string,int:characters)  // returns the first x characters of a string
 fn-id:25 |  fromright(string,int:characters)  // returns the last x characters of a string
 fn-id:26 |  trimright(string,int:totrim)  // trims a string at the end by totrim and returns that as a string
 fn-id:27 |  trimleft(string,int:totrim)  //  trims a string at the beginning by a given number returns the result as a new string
 fn-id:28 |  stringtohex(string)  // returns a hexed string from the givenstring
 fn-id:29 |  hextostring(hexstring)  // returns a string from a given hexstring
 fn-id:30 |  print(string,string:color)   // prints a string to the console,
 the color argument is optional colors can be given as the first character
 every color has a bright version
red = r
 blue = b
 bright blue = bb
 red = r etc
 fn-id:31 |  fileread(filepath)  // reads a file and returns the contents as a string
 fn-id:32 |  filewrite(filepath,string)  // returns status, writes a string to a file
 fn-id:33 |  filewriteasync(filepath,string)  // writes a string to a file as a new thread.
 fn-id:34 |  fileexists(filepath)  // returns a bool true if the filepath contains a file, and false if theres no file
 fn-id:35 |  filedelete(filepath)  // deletes a file at a given path
 fn-id:36 |  filemove(filepath,newpath)  // moves a file from a given path to another
 fn-id:37 |  filecopy(filepath,copiedpath)  // copies a file
 fn-id:38 |  dirmove(directorypath,)   // moves a directory to a new location
 fn-id:39 |  dirdelete(directorypath)  // deletes a directory
 fn-id:40 |  dircreate(directorypath)  // creates a directory
 fn-id:41 |  dirsize(directorypath)  // returns the size of a directory
 fn-id:42 |  formatbytes(bytesize)  // returns a B,KB,MB,GB,TB string
 fn-id:43 |  dirsizebytes(directorypath)  // returns the bytesize of a directory
 fn-id:44 |  listdir(directorypath,bool:fullpathasresult)   // returns a vector with all the files
 if the second argument is set to true all the entrees will have a full filepath
 if set false, or not given at all the entrees will only contain the filenames
 fn-id:45 |  filesize(filepath) // returns a kb/mb/gb floored number of the filesize
 fn-id:46 |  filesizebytes(filepath)  // returns the filesize in bytes
 fn-id:47 |  runwait(shellcommandstring)  // executes a shell command, returns the result
 this is a blocking function if the called program doesnt exit , relevant see run()
 fn-id:48 |  run(shellcommandstring) // executes a shell command, returns the status as a string. (none blocking) relevant : runwait()
 fn-id:49 |  round(numbervar,decimals) // returns a rounded number by the given decimals.
 fn-id:50 |  sleep(int:timeinms) //  will pause the thread for x ms seconds.
 can be usefull for lowering powerconsumption
 fn-id:51 |  cat(a,b,c,..) //  concatinates all arguments to eachother returns that as a new string.
 theres no limit on the ammount of arguments
 fn-id:52 |  string(a,b,c,..) //  concatinates all arguments to eachother returns that as a new string.
 theres no limit on the ammount of arguments
 fn-id:53 |  random(int:min,)     //  generates a random number by a minimum and maximum.
set decimal to 0 to get flat numbers
 fn-id:54 |  arraycontains(vector,string) //  returns a bool if a vector contains the given string.
 fn-id:55 |  arrayroll(vector,string)  // returns a new vec, LiFo , if the vector has a size of 6 is will remain the size the new entree will be inserted as 0 and the last one will be left out, each one will shift one spot.
 fn-id:56 |  arraypush(vector,string)  // pushes the string at the end of a vector returns a new vector
 fn-id:57 |  arraymerge(vector,vec,vec..)  // combines all entrees of all given vectors returns a new vector
 fn-id:58 |  arrayinsert(vector,)  // inserts the string to the vector and returns that as a new vector
 fn-id:59 |  arraysort(vector)  // sorts the vector by a alphabetic order and returns that as a new vector
 fn-id:60 |  arrayretain(vector,string) //  will remove the string from a vector, returns that as a new vector
 fn-id:61 |  arrayshuffle(vector)  // returns a shuffled vector as a new
 fn-id:62 |  arrayreverse(vector)  // reverses the vector returns that as a new
 fn-id:63 |  arraysearch(vector,string) //  will create a new vector with all entrees containing the given string
 fn-id:64 |  arrayfilter(vector,string) //  will create a new vector without all entrees containing the given string
 fn-id:65 |  httpgetcontent(ip,port,remotefile) //  will return the webcontent example :
 httpgetcontent("127.0.0.1",80,"/index.nc")
 fn-id:66 |  terminalinput(msgstring,defaultoption) //  the terminal will listen for given input,
 this function returns when the terminal gives a enter
 fn-id:67 |  splitselect(string,splitbydelimeter,int:vectorentree) //  will split a string with the given delimeter
 instead of returning a vector it will return the string by the given number
 fn-id:68 |  base64tofile(base64string,filepath) //  decodes base64 string and writes it as a file
 fn-id:69 |  filetobase64(filepath) //  reads a file and encodes it to base64
 fn-id:70 |  base64tostring(string) //  returns a decoded base64string
 fn-id:71 |  stringtobase64(base64string) //  decodes the string and returns that
 fn-id:72 |  tcplistener(ip,port) //  returns a listenersocket, can be used by other tcp***()
 fn-id:73 |  tcpaccept(listenersocket) //  returns a clientsocket when a client connects
 fn-id:74 |  tcpconnect(ip,port) //  returns a clientsocket
 can be used by tcpreceive
 fn-id:75 |  tcpdisconnect(clientsocket) // closes a clientsocket
 fn-id:76 |  tcpreceive(clientsocket) // returns a string if the clientsocket receives data
 fn-id:77 |  tcpsend(clientsocket,string) // sends a string to a clientsocket
 returns the status or send bytes
 fn-id:78 |  aabb_newbox(uniqueidentifierstring) // returns a object reference, usable for 3D collision checks
 fn-id:79 |  aabb_sizedbox(uniqueidentifierstring,scalex,scaley,scalez) // creates a 3d boundingbox by given scalesize
returns a object reference usable for 3D collision checks
 fn-id:80 |  aabb_setposition(idref,x,y,z) // sets a boundingbox to 3d coordinates ( no returns)
 fn-id:81 |  aabb_setrotation(idref,x,y,z) // sets a boundingbox to 3d coordinates ( no returns)
 fn-id:82 |  aabb_setscale(idref,x,y,z) // sets a boundingbox to 3d coordinates ( no returns)
 fn-id:83 |  aabb_addtogroup(idref,groupidref) // add a object to a collisiongroup
 fn-id:84 |  aabb_getgroup(groupidref) // returns a vector of all objects ina collisiongroup
 fn-id:85 |  aabb_removefromgroup(groupidref,idtoremove) // removes a entree from a group
 fn-id:86 |  aabb_getcollisions(targetid,groupid) // will return a vector of all entrees who are colliding in 3d with the targetid within a collisiongroup
 fn-id:87 |  aabb_removegroup(groupidref) // deletes a whole group.
 fn-id:88 |  decode_html_url(string) // decodes html content like arguments %12 etc
 fn-id:89 |  mod(number,maxnumber) // will keep the number in range, so lets say mod(10,8) will return 2
 fn-id:90 |  encrypt(datastring,passwordstring) // returns a encrypted string, can be used with decrypt(datastring,passwordstring)
 fn-id:91 |  decrypt(datastring,passwordstring) // returns a decrypted string, created by encrypt(str,pss)
 fn-id:92 |  arraynew() // returns a new array
 fn-id:93 |  arraynewsized(size) // returns a new array with empty strings by the given size
 fn-id:94 |  prefix(string) // returns the first character
 fn-id:95 |  suffix(string) // returns the last character
 fn-id:96 |  castray(rayid,vec:pos_a,vec:pos_b,f32:steps) // returns vec lenght creates a buffer vector , use with getraypoint(rayid,vecid)
 fn-id:97 |  getraypoint(rayid,step) // returns a vector with the position , by the given step of the ray
 fn-id:98 |  int_or(checkvarint,defaultint) // returns or if not a int
 fn-id:99 |  float_or(checkvarfloat,defaultfloat) // returns or if not a float
 fn-id:100 |  string_or(checkvar,default) // returns or if string is empty
 fn-id:101 |  newvar() // returns a new var
 fn-id:102 |  percentage(someammount,totalammount) // returns the percentage value
 fn-id:103 |  url(hostaddress,param,params..) // returns the the url string like http://site.com?parm1&param2&etc
 fn-id:104 |  objectgetrangebetween(object1,object2) // returns the range as a f32 using objects x y z propererties.
 fn-id:105 |  objectgetsiderangeobjectgetrange(side,range) // returns a f32;3 with the position, sides up/down/left/right #object requires .yaw .pitch
 fn-id:106 |  panicpanic(errormsg) // panics the program with a msg. Exits after
 fn-id:107 |  udpbindudpbind(ip,poort) // returns a socketID which can be used by udplisten(socketid) and udpsend(socketid,clientid,msg)
 fn-id:108 |  udplistenudplisten(udpsocketid) // returns a vec[0] for clientsocket and [1] for msgdata
 fn-id:109 |  udpsendudpsend(udpsocketid,clientsocketid,msgstring) // returns a error value=[ERROR] on failure
 fn-id:110 |  udpreplyudpreply(udpsocketid,clientsocketid,msgstring)    listen()              fn-id:111 |  socketaddresssocketaddress(ip,port)         udpsend() fn-id:112 |  arraypickrandomarraypickrandom(vec)         fn-id:113 |  terminaldisableraw() // disables raw mode terminal printing
 fn-id:114 |  terminalupdate(string) // prints a frame
 fn-id:115 |  printpos(string,color,x,y) // printtext printcolor charposx, charposy
 fn-id:116 |  terminalflush() // flushes the terminal : rawmode
 fn-id:117 |  terminalreset() // resets the terminal : rawmode
 fn-id:118 |  terminalenableraw() // enables raw mode terminal printing
 fn-id:119 |  terminalkey() // returns the pressed key as a string
````
