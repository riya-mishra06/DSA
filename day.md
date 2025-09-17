basic of js
Sum of 2 no

let a = 10;
let b = 20;
console.log("sum of 10 and 20 is" +(a+b));

Problem 1: Find Maximum in Array
let arr = [2, 8, 5, 1, 10, 3];
let max = arr[0];

for (let i = 1; i < arr.length; i++) {
    if (arr[i] > max) {
        max = arr[i];
    }
}
console.log("Maximum:", max); // 10

Problem 2: Reverse an Array
let arr = [1, 2, 3, 4, 5];
let reversed = [];

for (let i = arr.length - 1; i >= 0; i--) {
    reversed.push(arr[i]);
}
console.log("Reversed:", reversed); // [5,4,3,2,1]

Problem 3: Find Missing Number (1 to N)

Input: [1, 2, 4, 5] → Output: 3

let arr = [1, 2, 4, 5];
let n = 5; 
let total = (n * (n + 1)) / 2;
let sum = 0;

for (let i = 0; i < arr.length; i++) {
    sum += arr[i];
}
console.log("Missing Number:", total - sum); // 3

 Problem 4: Count Occurrences of Each Element
let arr = [2, 3, 2, 5, 3, 2];
let freq = {};

for (let i = 0; i < arr.length; i++) {
    let num = arr[i];
    if (freq[num]) {
        freq[num]++;
    } else {
        freq[num] = 1;
    }
}
console.log("Frequencies:", freq);
// { '2': 3, '3': 2, '5': 1 }
