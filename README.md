# min-max-sum

## Solution

`function miniMaxSum(arr) {
    arr.sort();
    let sum = 0;
    for (let i=0; i<arr.length; i++){
       sum = sum + arr[i]
    }
    const biggestNum = arr.pop();
    const smallestNum = arr.shift();
    const minSum = sum - biggestNum;
    const maxSum = sum - smallestNum;
    console.log(minSum, maxSum);
    return minSum, maxSum;
}`