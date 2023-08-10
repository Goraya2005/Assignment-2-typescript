# Assignment-2-typescript
"Assignment 2 TypeScript Repository" contains TypeScript solutions demonstrating unit consumption tax calculation, day-of-week determination,. These programs showcase TypeScript proficiency in implementing logic, handling inputs, and solving practical scenarios. Valuable for learning and practicing TypeScript concepts.





// Assignment for this week is:

//  - Write a program to convert the temperature from Celsius to Fahrenheit and vice verse.

var temp_Fahrenheit: number = 106;
var temp_Celsius: number = (temp_Fahrenheit - 32) * 5 / 9;    // Celsius = (Fahrenheit - 32) * 5 / 9
console.log(temp_Celsius); 

var temp_Celsius2: number = 42; 
var temp_Fahrenheit2: number = (temp_Celsius2 * 9 / 5) + 32; // Fahrenheit = (Celsius × 9/5) + 32
console.log(temp_Fahrenheit2);

//  - Write a program that calculates the percentage.

var studentName: string = "Naeem Goraya"
var studentMarks: number = 1098;
var totalMarks: number = 1100;
var studentMarksPecentage: number = (studentMarks / totalMarks) * 100;
console.log(`"The percentage of marks obtained by Mr. ${studentName}  is  " ${studentMarksPecentage}`);


//  - Write a program that converts given number of days in to weeks and days such as 17 days = 2 weeks and 3 days.

var totalDays: number = 359;
var totalWeeks: number = Math.floor(totalDays / 7);
var remainingDays: number = totalDays % 7;

if(totalWeeks == 0){
    console.log(`Number of weeks is Zero, however number of days are ${totalDays}`);
}
else if(totalDays == 0){
    console.log(`total number of weeks are ${totalWeeks} and remaining days are Zero`);
}
else {
    console.log(`total number of weeks are ${totalWeeks} and remaining days are ${remainingDays}`);
}


 

//  - Write a program that calculates the discount for a product based on its price. If the price is above $100, apply a 10% discount; otherwise, apply a 5% discount.

var productName: string = "Paper"
var productPrice: number = 188;
var discount10: number = productPrice * 10 / 100;
var discount5: number = productPrice * 5 / 100;

if (productPrice > 100){
    console.log(`The discounted price of ${productName} is $${productPrice - discount10}`);
}
else {
    console.log(`The discounted price of ${productName} is $${productPrice - discount5}`);
}

//  - Create a program that determines the category of a user-provided age. If the age is between 0 and 12, print "Child." If it's between 13 and 19, print "Teenager." Otherwise, print "Adult."

var theName: string = "Naeem Goraya";
var theAge: number = 76;
if(theAge > 12 && theAge < 20){
console.log(`Mr. ${theName} You are still a child.`);
}
else{
    console.log(`Mr. ${theName} You are an adult`);
}

//  - Write a program that takes temperature and check it. If it is cold then suggest the user to wear warm clothes and so on according to the weather.

var _Name: string = "Naeem Goraya";
var _temp: number = 10;

    if (_temp < 0) {
        console.log(`Mr. ${_Name}, It's extremely cold! Make sure to wear heavy winter clothing, including a coat, gloves, scarf, and hat.`);
    } 
    
    else if (_temp >= 0 && _temp < 10) {
        console.log(`Mr. ${_Name}, It's quite cold. Consider wearing a warm coat, gloves, and a scarf.`);
    } 
    
    else if (_temp >= 10 && _temp < 20) {
        console.log(`Mr. ${_Name}, It's chilly. A light jacket or sweater should be sufficient.`);
    } 
    
    else if (_temp >= 20 && _temp < 30) {
        console.log(`Mr. ${_Name}, It's a moderate temperature. A t-shirt and jeans would be comfortable.`);
    } 
    
    else {
        console.log(`Mr. ${_Name}, It's warm. You can wear light clothing like shorts and a t-shirt.`);
    }


//  - Write a program that checks if the given number is  divisible by 3 or 5 or both or not divisible by anyone show output accordingly.

var divideNumber: number = 6777655786;
var divide3: number = divideNumber % 3;
var divide5: number = divideNumber % 5;

if (divide3 == 0){
    console.log(` The Number ${divideNumber}, is divisible by 3`);
}

else if (divide5 == 0){
    console.log(` The Number ${divideNumber}, is divisible by 5`);
}

else if (divide3 == 0 && divide5 == 0){
    console.log(` The Number ${divideNumber}, is divisible by both 3 and 5`);
}

else {
    console.log(` The Number ${divideNumber}, is not divisible by both 3 and 5`);
}

//  - Write a program that checks if the given year is leap year or not.

var theYear: number = 2778;
if (theYear % 4 == 0){
    console.log(` The Year ${theYear}, is a Leap Year`);
}

else {
    console.log(` The Year ${theYear}, is not a Leap Year`);
}


//  - Develop a program that determines the day of the week. Ask the user for a number (1-7) and use nested if statements to print the corresponding day's name.

var dayNumber: number = 4; // Change this to a number between 1 and 7 for different results

if (dayNumber == 1) {
    console.log("The day corresponding to number 1 is Monday.");
} else if (dayNumber == 2) {
    console.log("The day corresponding to number 2 is Tuesday.");
} else if (dayNumber == 3) {
    console.log("The day corresponding to number 3 is Wednesday.");
} else if (dayNumber == 4) {
    console.log("The day corresponding to number 4 is Thursday.");
} else if (dayNumber == 5) {
    console.log("The day corresponding to number 5 is Friday.");
} else if (dayNumber == 6) {
    console.log("The day corresponding to number 6 is Saturday.");
} else if (dayNumber == 7) {
    console.log("The day corresponding to number 7 is Sunday.");
} else {
    console.log("Invalid day number.");
}








//  - Write a program that takes the number of units consumed by a user if it is greater than 100 then add 10% tax if greater than 200 then add 15% of tax so on up to if greater than 500 then add 25% of tax
// Where the tax amount will be calculated by the amount of bill.

var unitConsumed: number = 776;
var unitValue: number = 37;
var consumedValue: number = unitConsumed * unitValue

if (unitConsumed < 101){
    var tax1: number = consumedValue * 0 / 100;
    console.log(`The bill amount is Pak Rs. ${consumedValue + tax1}, where it includes the tax amount SPak Rs. ${tax1}`);
}

else if (unitConsumed > 100 && unitConsumed < 201){
    var tax1: number = consumedValue * 10 / 100;
    console.log(`The bill amount is Pak Rs. ${consumedValue + tax1}, where it includes the tax amount SPak Rs. ${tax1}`);
}

else if (unitConsumed > 200 && unitConsumed < 301){
    var tax1: number = consumedValue * 15 / 100;
    console.log(`The bill amount is Pak Rs. ${consumedValue + tax1}, where it includes the tax amount SPak Rs. ${tax1}`);
}
else if (unitConsumed > 300 && unitConsumed < 401){
    var tax1: number = consumedValue * 20 / 100;
    console.log(`The bill amount is Pak Rs. ${consumedValue + tax1}, where it includes the tax amount SPak Rs. ${tax1}`);
}
else if (unitConsumed > 400 && unitConsumed < 501){
    var tax1: number = consumedValue * 325 / 100;
    console.log(`The bill amount is Pak Rs. ${consumedValue + tax1}, where it includes the tax amount SPak Rs. ${tax1}`);
}
else {
    var tax1: number = consumedValue * 30 / 100;
    console.log(`The bill amount is Pak Rs. ${consumedValue + tax1}, where it includes the tax amount SPak Rs. ${tax1}`);
}

