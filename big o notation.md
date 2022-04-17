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
Linear Time:
<br></br>
Let's say we have the following variables:
```
T = Time
a = constant
b = constant
n = input
```
Now if we look at this equation: *T = an + b*
<br></br>
We can identify the fastest growing term is *n*.  This is because *a* and *b* are constants, and never change.  So the only thing that *can* grow is *n*.
<br></br>
If we take out the coefficients, we end up with: *T = ~~a~~n+~~b~~*.  That simplifies to *T = n* or (in Big O Notation) *T = O(n)*
___
Constant Time:
<br></br>
Let's say we have the following variables:
```
T = Time
a = constant
```
Now if we look at this equation: *T = a*
<br></br>
In this case, a never changes.  There is no growing term.
<br></br>
Because of this, it simplifies to *T = 1* or (in Big O Notation) *T = O(1)*
___
Quadratic Time:
<br></br>
Let's say we have the following variables:
```
T = Time
a = constant
b = constant
c = constant
n = input
```
Now if we look at this equation: *T = an<sup>2</sup> + bn + c*
<br></br>
We can identify the fastest growing term is *n<sup>2</sup>*.  This is because *a*, *b*, and *c* are constants, and never change.  *n* grows less quickly than *n<sup>2</sup>*.
<br></br>
If we take out the coefficients, we end up with: *T = ~~a~~n<sup>2</sup>+~~bn~~+~~c~~*.  That simplifies to *T = n<sup>2</sup>* or (in Big O Notation) *T = n<sup>2</sup>*
___
A small side note: If there is more than one input, you would keep both in Big O Notation.  For example:
```
T = Time
n = input #1
m = input #2
y = constant
```
If we look at this equation: *T = m<sup>2</sup> + m + n + y*.  If we take out the coefficients, we end up with: *T = m<sup>2</sup> + ~~m~~ + n + ~~y~~*.  This would simplify to *T = m<sup>2</sup> + n* or (in Big O Notation) *T = O(m<sup>2</sup> + n)*

## Rankings/Most Common Complexities (Best to Worst):
O(1)
<br></br>
O(log(n))
<br></br>
O(n)
<br></br>
O(n log(n))
<br></br>
O(n<sup>2</sup>), O(n<sup>3</sup>), O(n<sup>4</sup>)...
<br></br>
O(2<sup>n</sup>)
<br></br>
O(n!)
