## JavaScript Assigment completed

###### Note: To run these program's just copy the js code and paste it into index.js file and you can see the results.

1.  Create a variable.js file and declare variables and assign string, boolean, undefined and null data types, Display all the value with their data type.
    Program:

```javaScript
 // Declare and assign variables
var str = "Hello, world!"; // string
var bool = true; // boolean
var undef = undefined; // undefined
var nul = null; // null

// Display values and data types
console.log("str:", str, " (Type:", typeof str + ")");
console.log("bool:", bool, " (Type:", typeof bool + ")");
console.log("undef:", undef, " (Type:", typeof undef + ")");
console.log("nul:", nul, " (Type:", typeof nul + ")");
```

2.  Declare variables to store your first name, last name, marital status, country and age and display them using interploation method.
    Program:

```javaScript
const firstName = 'Rahul';
const lastName = 'Parmar';
const maritalStatus = 'Marid';
const country = 'India';
const aage = 28;
const userInfo = `Hi my name is ${firstName} my age is ${aage} and i am ${maritalStatus} and living in ${country}.`;
console.log(userInfo);
```

3.  Declare a varibale and assign string value to it and change all the string characters to capital letters using toUpperCase() method.
    Program:

```javaScript
 let str = ("hi my name is rahul parmar amd i am lerning java script");
console.log(str.toLocaleUpperCase());
```

4.  Declare a varibale and assign string value to it and check if the string contains a word Script using includes() method.
    Program:

```javaScript
let x = ("hi my name is rahul parmar amd i am lerning java script");
let y = x.includes("script")
console.log(y);
```

5.  Declare a varibale and assign string value to it and then split it into an array using split() method
    Program:

```javaScript
let A = ('hi my name is rahul parmar amd i am lerning java script');
let Arr = str.split(" ");
console.log(Arr);
```

6.  'Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon' split the string at the comma and change it to an array.
    Program:

```javaScript
let web = ('Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon')
let arr = web.split(",")
console.log(arr);
```

7.  Declare an array containing the multiple values and use lastIndexOf to determine the position of the first and last occurrence of a word "pw skills".
    Program:

```javaScript
const array = ['ram', 'sham', 'pw skills', 'chiku','neha','pw skills','megha'];
const ind = array.indexOf('pw skills');
//const ind = array.lastIndexOf('pw skills');
console.log(ind);
```

8.  Demonstrate the use of trim() to remove any trailing whitespace at the beginning and the end of a string.
    Program:

````javaScript
const srt ="       Hi My Name is Rahul        ";
console.log(srt.trim());```


09. Boolean value is either true or false.
    - Write three JavaScript statement example which provide truthy value.
    - Write three JavaScript statement example which provide falsy value.
Program:
```javaScript
 //  falsy value are : null, non , undefine ,0,"", false
if (0) {
    console.log(true)
} else
{
console.log(false)
};
//And truty values are:empty array also  a truthy value [] , true,apart from 0 all numbers are truthy, all strings  are truthy values
````

9.  Boolean value is either true or false. - Write three JavaScript statement example which provide truthy value. - Write three JavaScript statement example which provide falsy value.
    Program:

```javaScript
 //  falsy value are : null, non , undefine ,0,"", false
if (0) {
    console.log(true)
} else
{
console.log(false)
};
//And truty values are:empty array also  a truthy value [] , true,apart from 0 all numbers are truthy, all strings  are truthy values
```

10. Figure out the result of the following comparison expression first without using console.log(). After you decide the result confirm it using console.log() - 4 > 3 - 4 >= 3 - 4 < 3 - 4 <= 3 - 4 == 4 - 4 === 4 - 4 != 4 - 4 !== 4 - 4 != '4' - 4 == '4' - 4 === '4' - Find the length of python and jargon and make a falsy comparison statement.
    Program:

```javaScript
    - 4 > 3
    - 4 >= 3
    - 4 < 3
    - 4 <= 3
    - 4 == 4
    - 4 === 4
    - 4 != 4
    - 4 !== 4
    - 4 != '4'
    - 4 == '4'
    - 4 === '4'
    - Find the length of python and jargon and make a falsy comparison statement.

console.log(4 > 3); // true
console.log(4 >= 3); // true
console.log(4 < 3); // false
console.log(4 <= 3); // false
console.log(4 == 4); // true
console.log(4 === 4); // true
console.log(4 != 4); // false
console.log(4 !== 4); // false
console.log(4 != '4'); // false
console.log(4 == '4'); // true
console.log(4 === '4'); // false

var python = 'python';
var jargon = 'jargon';
console.log(python.length === jargon.length); // Falsy comparison statement
```

11. Use the Date object to do the following activities - What is the year today? - What is the month today as a number? - What is the date today? - What is the day today as a number? - What is the hours now? - What is the minutes now? - Find out the numbers of seconds elapsed from January 1, 1970 to now.
    Program:

```javaScript
//   - What is the year today?
let currentYear = new Date();
console.log(currentYear.getFullYear());
//- What is the date today?
let currentdate = new Date();
console.log(currentdate.getDate());
//- What is the month today as a number
let currentmonth = new Date();
console.log(currentmonth.getMonth());
//- What is the day today as a number?
let currentDay = new Date();
console.log(currentDay.getDay());
//- What is the hours now ?
let currentHours = new Date();
console.log(currentHours.getHours());
//- What is the minutes now?
let currentminutes = new Date();
console.log(currentminutes.getMinutes());
//- Find out the numbers of seconds elapsed from January 1, 1970 to now.
let Now = new Date(0);
console.log(Now);
```

12. Create a human readable time format using the Date time object - YYYY-MM-DD HH:mm - DD-MM-YYYY HH:mm - DD/MM/YYYY HH:mm
    Program:

```javaScript
let now = new Date();
// YYYY-MM-DD HH:mm format
let date1 = now.toISOString().slice(0, 19).replace("T", " ");
console.log("YYYY-MM-DD HH:mm format: " + date1);

// DD-MM-YYYY HH:mm format
let date2 = now.toLocaleDateString("en-GB") + " " + now.toLocaleTimeString();
console.log("DD-MM-YYYY HH:mm format: " + date2);

// DD/MM/YYYY HH:mm format
let date3 = now.toLocaleDateString("en-US").replace(/\//g, "/") + " " + now.toLocaleTimeString();
console.log("DD/MM/YYYY HH:mm format: " + date3);
```

13. Get user input using prompt(“Enter your age:”). If user is 18 or older , give feedback:'You are old enough to drive' but if not 18 give another feedback stating to wait for the number of years he needs to turn 18.
    Program:

```javaScript
 let birth = prompt("Enter your birth year")
    let now = new Date()
    let age = now.getYear() - birth + 1900

    if(age<18)
        console.log('You need to wait for the number of years to turn 18')
    else if(age>=18 && age<36)
        console.log('You are old enough to drive')
    else console.log('You can drive')
```

14. Even numbers are divisible by 2 and the remainder is zero. How do you check, if a number is even or not using JavaScript? Create a program which checks that the given number is even or odd.
    Program:

```javaScript
 const number = prompt("Enter a number: ");
    if(number % 2 == 0) {
    console.log("The number is even.");
    }

    else {
  console.log("The number is odd.");}
```

15. Write a program which can give grades to students according to theirs scores: - 80-100, A - 70-89, B - 60-69, C - 50-59, D - 0-49, F
    Program:

```javaScript
 - 80-100, A
    - 70-89, B
    - 60-69, C
    - 50-59, D
    - 0-49, F s
    var students = [['David', 80], ['Vinoth', 77], ['Divya', 88], ['Ishitha', 95], ['Thomas', 68]];

    var Avgmarks = 0;
    for (var i=0; i < students.length; i++) {
        Avgmarks += students[i][1];
        var avg = (Avgmarks/students.length);
      }

    console.log("Average grade: " + (Avgmarks)/students.length);

        if (avg < 49){
          console.log("Grade : F");
          }
        else if (avg < 59) {
                console.log("Grade : D");
                  }
        else if (avg < 69)
             {
                console.log("Grade : C");
        } else if (avg < 89) {
                console.log("Grade : B");
        } else if (avg < 100) {
                console.log("Grade : A");}
```

16. Check if the season is Autumn, Winter, Spring or Summer. If the user input is : - September, October or November, the season is Autumn. - December, January or February, the season is Winter. - March, April or May, the season is Spring - June, July or August, the season is Summer
    Program:

```javaScript
 var a = prompt("Enter a month Name please.");
   var b = "";

    switch(a){
        case 1: b = 1;
            break;
        case 2: b = 2;
            break;
        case 3: b = 3;
            break;
        case 4: b = 4;
            break;
        case 5: b = 5;
            break;
        case 6: b = 6;
            break;
        case 7: b = 7;
            break;
        case 8: b = 8;
            break;
        case 9: b = 9;
            break;
        case 10: b = 10;
            break;
        case 11: b = 11;
            break;
        case 12: b = 12;
            break;
        }

   if((a=='december') || (a=='january') || (a=='february')){
      document.write(" It is " + a + ", which is in winter season.")
    }

   if ((a == 'march') || (a == 'april') || (a == 'may')) {
      document.write(" It is " + a + ", which is in spring season.")
    }

   if((a=='june') || (a=='july') || (a=='august')){
      document.write(" It is " + a + ", which is in summer season.")
    }

   if((a=='september') || (a=='october') || (a=='november')){
     document.write(" It is " + a + ", which is in Autumn season.")
}
```

17. Write a program which tells the number of days in a month.
    Program:

```javaScript
 let a = prompt('Enter the month:');

   let b = a.charAt(0).toUpperCase();

   let c = a.slice(1, a.length).toLowerCase();

   let Month = (b + c);

   if ('January' === Month || 'March' === Month || 'May' === Month || 'July' === Month || 'Agust' === Month || 'October' === Month || 'December' === Month) {
       console.log(`${Month} has 31 days`)
       }
   else if ('February' === Month)
   {
       console.log(`${Month} has 28 days`);
   }
   else if ('April' === Month || 'June' === Month || 'September' === Month || 'November' === Month) {
       console.log(`${Month} has 30 days`)
   }
   else{
       console.log('Re-Enter');
   }
```

18. Write a program which tells the number of days in a month, now consider leap year.
    Program:

```javaScript
let a = prompt('Enter the month:');

   let b = a.charAt(0).toUpperCase();

   let d = a.slice(1, a.length).toLowerCase();

   let Month = (b + d);

   if ('January' === Month || 'March' === Month || 'May' === Month || 'July' === Month || 'Agust' === Month || 'October' === Month || 'December' === Month) {
       console.log(`${Month} has 31 days`)
       }
   else if ('February' === Month)
   {
       console.log(`${Month} has 28 days`);
   }
   else if ('April' === Month || 'June' === Month || 'September' === Month || 'November' === Month) {
       console.log(`${Month} has 30 days`)
   }
   else
    console.log('Re-Enter');

   function checkLeapYear(year) {

    const leap = new Date(year, 1, 29).getDate() === 29;
    if (leap) {
        console.log(year + ' is a leap year');
    } else {
        console.log(year + ' is not a leap year');
    }
    }

   // take input
   const year = prompt('Enter a year:');
   checkLeapYear(year);
```

19. Create a countries.js file and store the countries name into this file, create a file web_techs.js and store the popular web technology names into this file. Access both file in a third file named main.js
    Program:

```javaScript
// index.19.html (html code)
  <!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>How to emport and export JS files</title>
    <script src="./main.js" type="module"></script>
  </head>
  <body>
    hello world
  </body>
</html>
```

```javaScript

//countries19.js(js code)
export const countries =
  ['Albania',
  'Bolivia',
  'Canada',
  'Denmark',
  'Ethiopia',
  'Finland',
  'Germany',
  'Hungary',
  'Ireland',
  'Japan',
  'Kenya' ]

console.log(countries);   //  -> Albania
//console.log(countries[10])  //  -> Kenya

//let lastIndex = countries.length - 1;
//console.log(countries[lastIndex]) //  -> Kenya
```

```javaScript
//web_techs19.js(js code)
export const webTechs = [
  'HTML',
  'CSS',
  'JavaScript',
  'React',
  'Redux',
  'Node',
  'MongoDB'
] // List of web technologies

console.log(webTechs);        // all the array items
//console.log(webTechs.length) // => to know the size of the array, which is 7
//console.log(webTechs[0])     //  -> HTML
//console.log(webTechs[6])     //  -> MongoDB

//let lastIndex = webTechs.length - 1
//console.log(webTechs[lastIndex]) // -> MongoDB
```

```javaScript
//main19.js(js code)
import { countries } from "./countries19";
import { webTechs } from "./web_techs19";
console.log(countries,webTechs);
```

20. In the following shopping cart add, remove, edit items
    => const shoppingCart = ['Milk', 'Coffee', 'Tea', 'Honey'] - add 'Meat' in the beginning of your shopping cart if it has not been already added - add Sugar at the end of your shopping cart if it has not been already added - remove 'Honey' - modify Tea to 'Green Tea'
    Program:

```javaScript
const shoppingCart = ['Milk', 'Coffee', 'Tea', 'Honey'];
// Add 'Meat' at the beginning of the shopping cart if it has not been already added
if (!shoppingCart.includes('Meat')) {
  shoppingCart.unshift('Meat');
}

// Add 'Sugar' at the end of the shopping cart if it has not been already added
if (!shoppingCart.includes('Sugar')) {
  shoppingCart.push('Sugar');
}

// Remove 'Honey' from the shopping cart
if (shoppingCart.includes('Honey')) {
  shoppingCart.splice(shoppingCart.indexOf('Honey'), 1);
}

// Modify 'Tea' to 'Green Tea' in the shopping cart
if (shoppingCart.includes('Tea')) {
  shoppingCart[shoppingCart.indexOf('Tea')] = 'Green Tea';
}
console.log(shoppingCart);
```

21. In countries array check if 'Ethiopia' exists in the array if it exists print 'ETHIOPIA'. If it does not exist add to the countries list.
    Program:

```javaScript
const countries = ['USA', 'Canada', 'Australia', 'India', 'France'];

// Check if 'Ethiopia' exists in the countries array
if (countries.includes('Ethiopia')) {
  console.log('ETHIOPIA');
} else {
  // If 'Ethiopia' does not exist, add it to the countries array
  countries.push('Ethiopia');
}

console.log(countries);
```

22. The following is an array of 10 students ages:
    => const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24] - Sort the array and find the min and max age - Find the median age(one middle item or two middle items divided by two) - Find the average age(all items divided by number of items) - Find the range of the ages(max minus min) - Compare the value of (min - average) and (max - average), use abs() method
    Program:

```javaScript
const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24];
// Sort the array
ages.sort((a, b) => a - b);

// Find the min and max age
const minAge = ages[0];
const maxAge = ages[ages.length - 1];

// Find the median age
let medianAge;
if (ages.length % 2 === 0) {
  const middle1 = ages[ages.length / 2 - 1];
  const middle2 = ages[ages.length / 2];
  medianAge = (middle1 + middle2) / 2;
} else {
  medianAge = ages[Math.floor(ages.length / 2)];
}

// Find the average age
const sumAges = ages.reduce((acc, age) => acc + age, 0);
const averageAge = sumAges / ages.length;

// Find the range of ages
const range = maxAge - minAge;

// Compare min-average and max-average
const minAverageDiff = Math.abs(minAge - averageAge);
const maxAverageDiff = Math.abs(maxAge - averageAge);

// Output the results
console.log("Sorted Ages: ", ages);
console.log("Min Age: ", minAge);
console.log("Max Age: ", maxAge);
console.log("Median Age: ", medianAge);
console.log("Average Age: ", averageAge);
console.log("Range of Ages: ", range);
console.log("Min - Average: ", minAverageDiff);
console.log("Max - Average: ", maxAverageDiff);
```

23. Write a program to check that the number given by the user is a prime number or not.
    Program:

```javaScript
let num = parseInt(prompt("Enter a number: "));  // Get the number from the user and convert it to an integer

// Check if the number is less than or equal to 1
if (num <= 1) {
  console.log(num + " is not a prime number");
}

// Check for prime numbers
else {
  let prime = true;  // Assume that the number is prime initially

  // Check if the number is divisible by any number from 2 to num-1
  for (let i = 2; i < num; i++) {
    if (num % i === 0) {
      prime = false;  // The number is not prime
      break;
    }
  }

  // Print the result based on whether the number is prime or not
  if (prime) {
    console.log(num + " is a prime number");
  } else {
    console.log(num + " is not a prime number");
  }
}
```

24. Write a program to create two array "even" and "odd" having even and odd number between the 0 to 100 (0 and 100 included).
    Program:

```javaScript
let even = [];  // Array to hold even numbers
let odd = [];   // Array to hold odd numbers

// Loop through the numbers from 0 to 100 (inclusive)
for (let i = 0; i <= 100; i++) {
  if (i % 2 === 0) {
    even.push(i);  // If the number is even, add it to the "even" array
  } else {
    odd.push(i);   // If the number is odd, add it to the "odd" array
  }
}

// Print the arrays to the console
console.log("Even numbers between 0 and 100: " + even);
console.log("Odd numbers between 0 and 100: " + odd);
```

25. Body mass index(BMI) is calculated as follows: bmi = weight in Kg / (height x height) in m2. Write a function which calculates bmi. BMI is used to broadly define different weight groups in adults 20 years old or older.Check if a person is underweight, normal, overweight or obese based the information given below. - The same groups apply to both men and women. - Underweight: BMI is less than 18.5 - Normal weight: BMI is 18.5 to 24.9 - Overweight: BMI is 25 to 29.9 - Obese: BMI is 30 or more
    Program:

```javaScript
function calculateBMI(weight, height) {
  // Convert height to meters
  height = height / 100; // Assuming height is given in centimeters, converting to meters

  // Calculate BMI
  let bmi = weight / (height * height);

  // Categorize BMI
  let category;
  if (bmi < 18.5) {
    category = "Underweight";
  } else if (bmi >= 18.5 && bmi <= 24.9) {
    category = "Normal weight";
  } else if (bmi >= 25 && bmi <= 29.9) {
    category = "Overweight";
  } else {
    category = "Obese";
  }

  return { bmi: bmi, category: category };
}

// Example usage:
let weight = 70; // Weight in kg
let height = 170; // Height in cm

let result = calculateBMI(weight, height);
console.log("BMI: " + result.bmi.toFixed(2)); // Rounded to 2 decimal places
console.log("Category: " + result.category);
```

26. Write a program to print the table of any number given by the user. The format of the output should be smiliar to the below example-
    If the number given by the user is 2 then the output should look like this-
    2 _ 1 = 2
    2 _ 2 = 4
    2 _ 3 = 6 and so on till 2 _ 10 = 20.
    Program:

```javaScript
let number = parseInt(prompt("Enter a number to print its table:"));

// Check if user entered a valid number
if (isNaN(number)) {
  console.log("Invalid input. Please enter a number.");
} else {
  // Print the table of the number
  for (let i = 1; i <= 10; i++) {
    console.log(number + " * " + i + " = " + (number * i));
  }
}
```

27. Write a program to print all the prime number between 0 to 100 (0 and 100 included).
    Program:

```javaScript
function isPrime(n) {
  if (n <= 1) {
    return false;
  }

  for (let i = 2; i <= Math.sqrt(n); i++) {
    if (n % i === 0) {
      return false;
    }
  }

  return true;
}

// Loop through all numbers from 0 to 100 and print prime numbers
for (let i = 0; i <= 100; i++) {
  if (isPrime(i)) {
    console.log(i);
  }
}
```

28. Write a program to print the given patterns using the loops-

a. Print a triangle pattern, if the given input is 3 then the pattern should be similar to the given output

       *
       **
       ***

Program:

```javaScript
  let rows = 3;
   for (let i = 1; i <= rows; i++) {
  let pattern = "";
  for (let j = 1; j <= i; j++) {
    pattern += "*";
  }
  console.log(pattern);
}
```

b. Print a square pattern, if the input is 3 then the output should be similar to the given output

       ***
       ***
       ***

Program:

```javaScript
 let rows = 3;
   let cols = 3;

  for (let i = 1; i <= rows; i++) {
  let pattern = "";
  for (let j = 1; j <= cols; j++) {
    pattern += "*";
  }
  console.log(pattern);
}
```

c. Print a pyramid pattern, if the input is 3 then the output should be similar to the given output

         *
        ***

---

Program:

```javaScript
let rows = 3;
   for (let i = 1; i <= rows; i++) {
  let pattern = "";
  for (let j = 1; j <= rows - i; j++) {
    pattern += " ";
  }
  for (let k = 1; k <= 2 * i - 1; k++) {
    pattern += "*";
  }
  console.log(pattern);
}
```

29. Write a javascript program which takes the input of filename as string and prints the extension of the file in the console.
    Program:

```javaScript
let filename = "example.js";
let extension = filename.split(".").pop();
console.log(extension);
```

30. Create a simple calculator program in JavaScript which can perform the addition, substraction, multiplication and division on given numbers.
    Program:

```javaScript
let num1 = parseFloat(prompt("Enter the first number: "));
let num2 = parseFloat(prompt("Enter the second number: "));
let operation = prompt("Enter the operation (+, -, *, /): ");

let result;

if (operation === "+") {
  result = num1 + num2;
} else if (operation === "-") {
  result = num1 - num2;
} else if (operation === "*") {
  result = num1 * num2;
} else if (operation === "/") {
  result = num1 / num2;
} else {
  console.log("Invalid operation.");
}
console.log("Result: " + result);
```
