# Fibonacci and Rust
I used this project (calculating Fibonacci numbers) to explore a bit with Rust. Here are some of the language features that I learned about:  

* ```for``` loops
* Statements vs. expressions
* Function returns (expressions)
* ```checked_add``` to prevent overflow
* Option enum (returned from ```checked_add```)
* Pattern matching on Option
* Result enum (to return error rather than panic)
* ```.expects``` with Result
* Pattern matching on Result

An upcoming article will walk through using these while building the application. Intermediate steps are saved with the branches of the repository: 

* 01-creation  
Project state after ```cargo new fib```.
* 02-basic  
Basic implementation of Fibonacci (no error checking). Includes returning a value from a function.
* 03-mainloop  
Adding a loop to main to make it easier to run through various values. Shows 'panic' on overflow.
* 04-checkedadd  
Using ```checked_add``` to prevent overflow. Includes pattern matching on Option.  
*Note: this version does not 'panic', but it does not return '0' if the value overflows.*
* 05-result  
Returning a Result enum from the Fibonacci function. Uses '.expects' in the main loop.  
*Note: this version panics on overflow.*
* 06-matchresult  
Pattern matching on the Result in the main loop. This will show the correct value or a message that the overflow has occurred. This version does *not* panic.

Overall, this was a good way to experiment with a language that I have minimal experience with.