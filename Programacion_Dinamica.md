# Programacion Dinamica

## Ejercicio factorial

```
function factorial(x)
{
let memo={};
  if (x === 0)
 {
    return 1;
 }
 var n1;
 if(memo[x-1]){
   n1=memo[x-1]
 }else{
   n1=factorial(x-1)
 }

  return x * n1;
}

```

## Ejercicio Divisor Game

```

var divisorGame = function(N) {
    return N%2===0;
};

```
## Ejercicio Best time to Buy and Sell

```

var maxProfit = function(prices) {
    if (prices.length === 0){
      return 0;   
    }
    let maxProfit = 0, j = 1, currentMin = prices[0];
    while(j < prices.length) {
        maxProfit = Math.max(prices[j] - currentMin, maxProfit);
        currentMin = Math.min(prices[j], currentMin);
        j++;
    }
    return maxProfit;
};

```
