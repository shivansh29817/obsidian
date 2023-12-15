
##### Ways to print in Javascript -- js console API
  
```
console.log("HELLO ",4+6,"world");          // used to print something on console.

document.write("hello not human");          // used to write something on page.

console.warn("This is warning");            // used to give warning on the console.

console.error("This is error");             // used to lock error on console.

console.clear()                             // used to clear the console.

alert("me");                                // used to give alert on page.

//    dot (.) --> class  , hash (#) --> id.

  
```

---

#### Data type

- Integer
```
var num1 = 45;
var num2 = 36;
console.log( num1 , num2);
```

- String
```
var str = "Hello not human";
console.log(str);
```
  
- Objects
```
var obj = {
	badge : 99,
	white : 444
}
console.log(obj);
```
  
- Booleans
```
var m = true;
var n = false;
console.log(m,n);
```
  
- Null
```
var h = null;
console.log(h);
const a = 3, b = 2;
console.log(a > b);  
```

###### There are two types of data types

- Primitive --> undefined ,null ,number ,string , booleans ,symbol
- Reference --> arrays ,object

---
#### Array

```
let arr = [1,2,3,4,5,"not human"];
console.log(arr);
```
  
**Include function**
```
var list = ["badge","white","nothuman"]
var name = "nothuman"
if(list.includes(name)) {
	console.log("yes");
}
else console.log('no');
```
  
 **Push function**
```
var name = []
name.push(2);
console.log(name);
```
  
---

#### For in loops 

```
let obj={
	badge :  99,
	white   :   444
}
for(let a in obj){
	console.log("Name"+ a + "no" +  obj[a]);
}
```
  
---

##### Basic functions 

```
var name = "nothuman";
console.log( name.length); ;
```
  
- Slicer -- `word.slice(__,__)`

```
var name = "Nothuman"
console.log(name.slice(0,5));
```

- Change in upper or lower case 

```
var name = "Nothuman";
name.toUpperCase();
name.toLowerCase();
```

- **Random number generator** # 16 decimal place 

```
var n = Math.random();
n = n * 100                        //100 is the range of the Number
n = Math.floor(n)
console.log(n);
//  OR
console.log(Math.floor(Math.random()*100));
```

---

#### Js in HTML 

```
<body onload="alert('hello');">

<script>
	document.querySelector("h1").innerHTML = "Good bye";        
</script>
```

- For selecting the specefic element                                    

```
document.getElementbyTagName("li")[2].style.colour = "purple"          

document.getElementbyTagName("li").length                              

document.getElementbyClassName("li")[0].style.colour = "red"          

document.getElementbyId("title")                                      

document.getElementbyId("title").innerHTML = "Hello" 'or' "<em>Hello</em>"

document.getElementbyId("title").innerHTML                                      
// it gives whole element

document.getElementbyId("title").textContent
// it gives only inside text  written

document.querrySelector("a").attributes
// it gives all the anchor tag attributes

document.querrySelector("a").getAttribute("href") 
// it gives you only the link

document.querrySelector("a").setAttribute("href", https:// www.bing.com)   
// it will change the prev. href into second parameter

```

---

```
document.querrySelector("h1") 
//or
document.querrySelector("#title")     //for Id
document.querrySelector(".btn")       //for Class


document.querrySelector("li.item")          
// points to anchor tag inside list item (Class)

document.querrySelector("#list a")   
// points to anchor tag inside list item (Id)

document.querrySelector("#list .item")         
// it will give only first element   'or'

document.querrySelectorAll("#list .item")    
// it will give all element item Classes inside list Id

document.querrySelectorAll("#list .item")[2]   
// it will give the specified element

document.querrySelector("button").classList;     
// it will give the list of classes

document.querrySelector("button").classList.add("invisible")    
// it will add the invisible class

document.querrySelector("button").classList.remove("invisible")    
// it will remove the invisible class

document.querrySelector("button").classList.toggle("invisible")     
// if enable then remove ,vice versa the invisible class
```

#### Event Listener

```
document.querrySelector(.class).addEventListener("Click",function)        
// it will call the fun on the click for all querrySelector            


$0.addEventListener("Click",functio (){                
// it will call the fun when $0 element get clicked and will show the alert

	alert('i got clicked');
});             'or'

$0.addEventListener("Click", action);   
// it is another way of writing the function


function action() {
	alert('i got clicked'); 
}
document.querrySelectorAll(.Id).addEventListener("Click", functoin (){
	console.log(this);
});                    
// it will print the selected id object


document,addEventListener("Keypress",function(){                
	alert("kety is pressed");
}
// it will call the fun when a key is pressed

```

---


### For playing Audio file

```
var song1 = new Audio("file_name.mp3");       
// it will play the audio file
song1.play();
```
  

