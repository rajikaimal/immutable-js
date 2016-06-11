<a href="https://promisesaplus.com/">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/JavaScript-logo.png/768px-JavaScript-logo.png" width="100" align="right" />
</a>

# immutable-js

List of immutable functions in JavaScript

- [1.0](#1.0) <a name='1.0'></a> slice

  ```js
  // extracts certain section of a string and return a new string
  // doesn't mutate the original string
  
  var name = 'Stephanie Hwang'
  var first = name.slice(0, 8)
  
  console.log(name) //Stephanie Hwang
  console.log(first) //Stepanie
  console.log(name) //Stephanie Hwang
  ```

- [2.0](#2.0) <a name='1.0'></a> concat

  ```js
  // concatenate two strings
  // returns a new string
  
  var first = 'Stephanie'
  var last = ' Hwang'
  
  var fullName = first.concat(last);
  
  console.log(first) //Stephanie
  console.log(last) //Hwang
  console.log(fullName) //Stephanie Hwang
  console.log(first) //Stephanie
  console.log(last) //Hwang
  
  ```
  
- [3.0](#3.0) <a name='1.0'></a> replace

  ```js
  // replaces matching section of a the string which is explicitly passed to replace function
  
  var re = /Harry/gi
  var str = "Harry is a memeber of gryffindor."
  var newstr = str.replace(re, "Hermione")
           
  console.log(str) //Harry is a memeber of gryffindor.
  console.log(newstr) //Hermione is a memeber of gryffindor.
  console.log(str) //Harry is a memeber of gryffindor.
  ```
  
- [4.0](#4.0) <a name='1.0'></a> split

  ```js
  //split a given string into an array of strings
  
  var str = "Apples are round, and apples are juicy.";
  var newstr = str.split(" ", 2);
           
  console.log(str) //Apples are round, and apples are juicy.
  console.log(newstr) //['Apples', 'are']
  console.log(str) //Apples are round, and apples are juicy.
  ```
- [5.0](#5.0) <a name='1.0'></a> substr

  ```js
  //extracts part of a string
  
  var str = "Ten points for gryffindor"
  var newstr = str.substr(0, 3)
           
  console.log(str) //Ten points for gryffindor
  console.log(newstr) //Ten
  console.log(str) //Ten points for gryffindor
  ```
  
- [6.0](#6.0) <a name='1.0'></a> substring

  ```js
  //extracts part of a string
  
  var str = "Ten points for gryffindor"
  var newstr = str.substring(0, 3)
           
  console.log(str) //Ten points for gryffindor
  console.log(newstr) //Ten
  console.log(str) //Ten points for gryffindor
  ```

- [7.0](#7.0) <a name='1.0'></a> toLocaleLowerCase

  ```js
  //converts string to lowercase by keeping it's current locale
  
  var str = "Ron loves Hermionie"
  var newstr = str.toLocaleLowerCase()
           
  console.log(str) //Ron loves Hermionie
  console.log(newstr) //ron loves hermionie
  console.log(str) //Ron loves Hermionie
  ```
  
- [8.0](#8.0) <a name='1.0'></a> toLocaleUpperCase

  ```js
  //converts string to uppercase by keeping it's current locale
  
  var str = "Ron loves Hermionie"
  var newstr = str.toLocaleUpperCase()
           
  console.log(str) //Ron loves Hermionie
  console.log(newstr) //RON LOVES HERMIONIE
  console.log(str) //Ron loves Hermionie
  ```
  
- [9.0](#9.0) <a name='1.0'></a> toString

  ```js
  //converts type to represent string
  
  var phone = 124587921
  var phonestr = phone.toString()
           
  console.log(phone) //124587921
  console.log(phonestr) // "124587921"
  console.log(phone) //124587921
  ```
  
- [10.0](#10.0) <a name='1.0'></a> toLowerCase

  ```js
  //converts string to lowercase
  
  var str = "Ron loves Hermionie"
  var newstr = str.toLocaleLowerCase()
           
  console.log(str) //Ron loves Hermionie
  console.log(newstr) //ron loves hermionie
  console.log(str) //Ron loves Hermionie
  ```
  
- [11.0](#11.0) <a name='1.0'></a> toUpperCase

  ```js
  //converts string to uppercase
  
  var str = "Ron loves Hermionie"
  var newstr = str.toLocaleUpperCase()
           
  console.log(str) //Ron loves Hermionie
  console.log(newstr) //RON LOVES HERMIONIE
  console.log(str) //Ron loves Hermionie
 
- [12.0](#12.0) <a name='1.0'></a> map

  ```js
  //iterates through an array
  
  var names = ['rajika', 'stephanie', 'taeyeon']
  names.map(function(name) {
      console.log(name)
  })
  //es6 syntax, arrow function
  //names.map((name) => {
  //  console.log(name)
  //})
  console.log(names)
