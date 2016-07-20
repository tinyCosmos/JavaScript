#JavaScript
######1. SPLIT splits a String bject into an array of strings
```JavaScript
var str = "How are you doing today?";
var res = str.split();      //["How are you doing today?"]
var res = str.split("");    //["H", "o", "w", " ", "a", "r", "e", " ", "y", "o", "u", " ", "d", "o", "i", "n", "g", " ", "t", "o", "d", "a", "y", "?"]
var res = str.split(" ",3); //["How", "are", "you"]
var res = str.split("o");   //["H", "w are y", "u d", "ing t", "day?"]
```
//REVERSE reverses an array
var myArray = ['one', 'two', 'three'];
myArray.reverse(); // ['three', 'two', 'one']

//JOIN joins all elements of an array into a string
var a = ['Wind', 'Rain', 'Fire'];
a.join();      //'Wind,Rain,Fire'
a.join(', ');  //'Wind, Rain, Fire'
a.join(' + '); //'Wind + Rain + Fire'
a.join('');    //'WindRainFire'

//REPLACE replaces with a new string
var str = "Visit Mom!";
var res = str.replace("Mom", "Dad");  //Visit Dad!

var myString = 'abc123.8<blah>';
myString = myString.replace(/\D/g,'');      //1238

var myString = 'abc123.8<blah>';
myString = myString.replace(/[0-9]/g, '');  //abc.<blah>

//TOLOWERCASE returns the calling string value converted to lowercase
var str = "Hello World!";
var res = str.toLowerCase();  //hello world!

//SLICE returns the selected elements in an array, as a new array object
var fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
var citrus = fruits.slice(1, 3);  //Orange,Lemon

//TOUPPERCASE converts a string to uppercase letters
var str = "Hello World!";
var res = str.toUpperCase();  //HELLO WORLD!

//SUBSTRING returns a subset of a string between one index and another, or through the end of the string.
var str = "Hello world!";
var res = str.substring(1, 4);  //ell - index 1, 2 and 3

//SUBSTR extracts parts of a string, beginning at the character at the specified position, and returns the specified number of characters
var str = "Hello world!";
var res = str.substr(1, 4);  //ello - index 1, 2, 3 and 4

//SPLICE changes the content of an array by removing existing elements and/or adding new elements.
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(2, 0, "Lemon", "Kiwi");  //Banana,Orange,Lemon,Kiwi,Apple,Mango

//INDEXOF returns the position of the first occurrence of a specified value in a string
var str = "Hello world, welcome to the universe.";
var n = str.indexOf("e");  //1

//FILTER creates a new array with all elements that pass the test implemented by the provided function
function isBigEnough(value) {
  return value >= 10;
}
var filtered = [12, 5, 8, 130, 44].filter(isBigEnough);  //filtered is [12, 130, 44]

//SORT sorts the elements of an array in place and returns the array
var fruit = ['cherries', 'apples', 'bananas'];
fruit.sort();  // ['apples', 'bananas', 'cherries']

var points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return a-b}); //[1,5,10,25,40,100]

//CHARAT returns the character at the specified index in a string
var str = "HELLO WORLD";
var res = str.charAt(0); //H

//FROMCHARCODE converts a Unicode number into a character
var res = String.fromCharCode(65); //A

//CHARCODEAT returns the Unicode of the character at the specified index in a string
var str = "HELLO WORLD";
var n = str.charCodeAt(0); //72

//Math.round() Round a number to the nearest integer
Math.round(2.5);  //3

//Math.floor() Round a number downward to its nearest integer
Math.floor(1.6);  //1
