## **Comments**
* **in-line comment** : 
```
eg : var n = 5; //this is an inline comment
```

* **multi-line comment** : 
``` 
 /*
var n = 5;
var d = 10;
aefdsf
fdf
dfggdfv
sdfvf
*/
```
## **Data types and variables**
1) **undefined** : Something that hasn't been defined
    
2) **null** : u have defined something and that someting is **nothing**

3) **Boolean** : true or false

4) **symbol** : Immutable primitive value that is unique.
    
 5) **numbers**

6) **object** : Can store different key value pair

## **Declare variable**
1) using **var** 
* variable can be used throughout the program.
* eg : var n = "Fruits";

2) using **let**
* Can only be used within the scope of where u decleared.
* eg : let n = "Fruits";

3) using **const**
* A variable which can never change.
* eg :  const pi = 3.14;

----------------------------------------------
----------------------------------------------

**console.log(variable_name)** : allows u to see things in console
```
eg :-
        var a = 2;
        consol.log(a);
        a = 10;
        console.log(a);

        Output
        ------
        2
        10
```

## **Escaping literal Quotes**
How to use quotes in a string.
```
var s = "I am a "good boy" who lives near your "House"";
```

The above stament will cause an error. So to solve it we can use an escape character

```
var s = "I am a \"good boy\" who lives near your \"House"";

Output
------
I am a "good boy" who lives near your "House"
```


**NOTE**:-
You can write a string in a single quote('') and can use double quote("") inside the sting

```
eg : var s = 'I am a "good boy" who lives near your "House"'

Output
------
I am a "good boy" who lives near your "House"
```

If u use backticks(`), then you can use both single quotes(') and double quotes(") in the string. Strings made using these are called templete strings.

```
eg : var s = `I 'am' a "good boy" who 'lives' near your "House"`

Output
------
I 'am' a "good boy" who 'lives' near your "House"
```
You can also use backticks for inserting values into a string directly

```
eg : `Items(${2 + 5})`

${} : lets u add numbers dirctly into a string.

Output
------
Items(7)
```
We can also write multi line string with backticks.

```
eg : 
     `hello 
      world
      sdhbsdj
      dshdcbsjdcbdjhc
      shsch
      `
```

## Double equal to (==) and triple equal to(===)

* **Double equal to (==)** : converts both value into the same type 

```
eg : 3 == '3'

Output
------
True
```
* **Triple equal to (===)** : Do not convert both value into the same type.

```
eg : 3 === '3'

Output
------
False
```
**Note** : It is same for not equal to. We use !== instead of !=.

## [Funtions](https://github.com/Ajallen14/Javascript/blob/main/funtions.html)

Keyword for creating a function is '**funtion**'

**Rules for naming a function** :-
- Can't use special words. eg : funtion
- Can't start with a number.
- Can't use special character except: $, _ .

(Camelcase is recomended)

Funtions are also treated as **values** in the javascript.

## [Object]()

Objects group multiple values together.

```
const prod = {
                pro_name : 'Socks',
                price : 10000,
            };
```

Here name and price are known as **property**. Using property we can access specific values in the object.

```
console.log(prod.pro_name);
```
This will access the value associated with the name 'pro_name'.

If you wanna change the value of a property u can change it using
```
prod.name = 'Cotton Socks';
console.log(prod.name)
```
The name will change from 'Socks' to 'Cotton socks'.
To remove a property from the object use the keyword 'delete'
```
delete prod.price;
```
**Bracket Notation** lets us use properties that don't work with dot notation.

```
const prod = {
                name : 'Socks',
                ['delivery-time'] : '2 days',
            };
```
If it is a string between the brackets, the brackets are optional
```
const prod = {
                name : 'Socks',
                'delivery-time' : '2 days',
            };
```
**Nested Object**
```
const prod = { // Object
                name : 'Socks',
                price : 10000,
                ['delivery-time'] : '2 days',
                rating : { //nested Object
                    stars : 4.5,
                    count : 87,
                }
            };
```

**Local Storage**
Only supports string

```
localStorage.setItem('msg', 'Hellooo');
```

**Properties and Methods**

* length : finds the lenth of the string
```
console.log('hello'.length);

OUTPUT
------

5
```

* **toUpperCase** : makes a string to Upper case
```
 console.log('hello'.toUpercase);

 OUTPUT
------

HELLO
```

**Auto-Boxing**

JS automatically wraps a string in speacial object first and then this object is used for further nedds. It is done automatically. It also works with other values like numbers and boolean but it does not work with null and undefined.
eg :

```
console.log('hello'.length);
                |
                |
                +-----> +--------+
                        | hello  |
                        +--------+
                        Special Object
```

**Destructuring**
* It is an easier way to take properties out of an object.
* If the variable name and property name is same. We can write it as below
```
const message = object1.message;

is same as writing:-
 
const {message} = object1
```
Here the it will take the 'message' property out of the 'object1' and save it in a variable called message.

**Shorthand Property**
If the property and variable name are same we can write it once.

eg:
```
const object1 = {
    message : message  ------> Variable
};      |
        +-----> Property

It takes whatever is in the 'message' variable and substitute into the code

is same as writing:-

const object1= {
    message
};
```