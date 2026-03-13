# JS coding questions: my practice note

## Fibonacci
- `next number = previous two numbers sum.`

### Algorithm
1. Start
2. Set first = 0, second = 1
3. Print first and second
4. Repeat until n numbers:
      next = first + second
      print next
      first = second
      second = next
5. End

```
function fibonacci(n){
    
    let first = 0 ;
    let second = 1 ;
    let next ;
    console.log(first)
    console.log(second)

    for(let i  = 2 ; i < n ; i ++){
        next = first + second;
        console.log(next);
         first = second;
         second = next;
    }
   }

fibonacci(8)

```


