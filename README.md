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


######################################################################################################################################################################

# Quarter of the year
### DESCRIPTION
###### Given a month as an integer from 1 to 12, return to which quarter of the year it belongs as an integer number.

######For example: month 2 (February), is part of the first quarter; month 6 (June), is part of the second quarter; and month 11 (November), is part of the fourth quarter.
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
