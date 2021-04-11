# *Tables*
## *to create a table in html follow these steps.*
+ ## *use this element \<table> \</table>*
+ ## *inside the table element use \<tr>  \</tr> to indicate the start of each row of the table.*
+ ## *inside each row element use \<td>any data\</td>.*
+ ## *to add a header use \<th>\</th>*

```
<table>
<tr>
<th></th>
<th>header of first column</th>
<th>header of second column</th>
</tr>
<tr>
<th>header of first row</th>
<td>first row with first column element</td>
<td>first row with second column element</td>
</tr>
</table>
```

# *objects*
## *we create objects by two ways:*
1. ## *creating object using literal notation and adding properties and methods:*

```
const objectName= {                                     // creating object
    property1:'anything',                               // adding properties   (variables)
    property2:20,
    methodName:function(){                              // adding methods  (function)
        any code
    },
}

objectName.propertyName='anything';                    // adding or updating properties

objectName.methodName = function(){                    // adding methods (function)
    any code
};
```


2. ## *creating blank object using constructor notation and adding properties and methods:*

```
const objectName = new Object();                       // creating a blank object

objectName.propertyName= 'anything';                   // adding or updating property 
objectName.propertyName=20;            

objectName['propertyName']= 'anything';                // another way of adding or updating property but not methods

delete objectName.propertyName;                        // deleting properties (variables)

objectName.methodName = function(){                    // adding methods (function)
    any code
};
```


## *arrays are special type of objects, and you can use both arrays and objects to create complex data, both of them can contain the other.*

# [back](../README.md)