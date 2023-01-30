# Codewars-js-problems

## the first problem
#### Sum of two lowest positive integers
##### DESCRIPTION:
###### Create a function that returns the sum of the two lowest positive numbers given an array of minimum 4 positive integers. No floats or non-positive integers will be passed.
###### For example, when an array is passed like [19, 5, 42, 2, 77], the output should be 7.
###### [10, 343445353, 3453445, 3453545353453] should return 3453455.

## the code:
```
function sumTwoSmallestNumbers(numbers) {  
  //Code here
  var ordered = numbers.sort(function(a,b){return a-b;});
  var result=0;
  for(i=0; i<ordered.length; i++){
    if(i==0){
      result+=ordered[0];
    }
    if(i==1){
      result+=ordered[1];
    }
  }
  return result;
}
```


#################################################################################################

# Quarter of the year
### DESCRIPTION
###### Given a month as an integer from 1 to 12, return to which quarter of the year it belongs as an integer number.
###### For example: month 2 (February), is part of the first quarter; month 6 (June), is part of the second quarter; and month 11 (November), is part of the fourth quarter.
## the code:
```
const quarterOf = (month) => {
    // Your code here

      if(month == 1 || month == 2 || month == 3){
        return 1;
      }else if (month == 4 || month == 5 || month == 6){
        return 2;
      }else if (month == 7 || month == 8 || month == 9){
        return 3;
      }else if (month == 10 || month == 11 || month == 12){
        return 4;
      }
    }

console.log(quarterOf(7));
```
#################################################################################################

# Multiplication table for number
### DESCRIPTION
###### Your goal is to return multiplication table for number that is always an integer from 1 to 10.

###### For example, a multiplication table (string) for number == 5 looks like below:
```
1 * 5 = 5
2 * 5 = 10
3 * 5 = 15
4 * 5 = 20
5 * 5 = 25
6 * 5 = 30
7 * 5 = 35
8 * 5 = 40
9 * 5 = 45
10 * 5 = 50
P. S. You can use \n in string to jump to the next line.
```

###### Note: newlines should be added between rows, but there should be no trailing newline at the end. If you're unsure about the format, look at the sample tests.

## the code:
```
sul 1:

function multiTable(number) {
  // good luck
var msg = "";
for(let i = 1 ; i<=10 ; i++){
  var ans = i * number;
  msg += `${i} * ${number} = ${ans}\n`;
}
return msg.trim('\n')
}

sul 2:

function multiTable(number) {
  let table = '';
  for(let i = 1; i <= 10; i++){
    table += `${i} * ${number} = ${i*number}\n`
  }
  return table.slice(0, -1)
}

sul 3:

const multiTable = n => Array.from(Array(10), (e, i) => `${++i} * ${n} = ${i * n}`).join('\n');
```
####################################################################################################

# Remove String Spaces
### DESCRIPTION
###### Simple, remove the spaces from the string, then return the resultant string.
## the code:
```
function noSpace(x){
return  x.replaceAll(' ', '');
}
```
