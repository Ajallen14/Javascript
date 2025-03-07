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

```
NOTE:-
You can write a string in a single quote('') and can use double quote("") inside the sting

eg : var s = 'I am a "good boy" who lives near your "House"'

Output
------
I am a "good boy" who lives near your "House"

If u use backticks(`), then you can use both single quotes(') and double quotes(") in the string.

eg : var s = `I 'am' a "good boy" who 'lives' near your "House"`

Output
------
I 'am' a "good boy" who 'lives' near your "House"
```