# Big O Notation

### Big O Notation is [asymptotic analysis](https://www.geeksforgeeks.org/analysis-of-algorithms-set-1-asymptotic-analysis/#:~:text=Asymptotic%20Analysis%20is%20the%20big,increases%20with%20the%20input%20size.).
#### This means we analyze the behavoir of a function as its input increases toward infinity. ♾️
The main focus is on how the input affects function performance.  Because of this, we don't really care too much about constants.  We are also more focused on worst case scenarios (ex. if the input is *really* big).

### But why do this?

Well, realistically, the time it takes for a computer to run a function is dependent on *lots* of factors, like computer speculations, concurrent programs running, etc.

Big O Notation provides a more consistent way to measure function performance, by seeing how the runtime of a function grows with larger inputs.

## Constant Time: O(1) ✔️
Constant time does not care about the size of input (n).  Essentially, memory is just being accessed.  The notation for constant time is O(1), because it does not change with the input.
<br></br>
<img src='https://arturmeyster.com/content/images/2015/02/constant-time-1.png' alt='constant time graph'></img>

## Linear Time: O(n) 👌
Linear time increases in a linear fashion as input (n) increases.
<br></br>
<img src='https://arturmeyster.com/content/images/2015/02/linear-time.png' alt='linear time graph'></img>

## Quadratic Time: O(n<sup>2</sup>) 🙅‍♀️
Quadratic time increases exponentially as input (n) increases. *yikes*
<br></br>
<img src='https://arturmeyster.com/content/images/2015/02/quadratic-time.png' alt='quadratic time graph'></img>

## How do you find O(n)?
Generally speaking, you:
1. Find the fastest growing term (n)
2. Take out the coefficient

### Some examples:
#### Linear Time:
