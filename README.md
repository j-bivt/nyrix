# tarsk syntax update
The final syntax for the terminal in/out commands are now done.

They look something like this:

```# example syntax of io, also did you know comments work?
# output
io term out "hello world" [d] # print "hello world" in plain, default text.
io term out "hello world" [l] # print "hello world" in bright green text, for logging.
io term out "hello world" [e] # print "hello world" in bright red, for showing errors AND warnings.

# bonus: you can reference variables
io term out @myVar [d]

# now inputs
io term in "what is 2 + 2? > " @ans # the @ symbol means variable, after the user inputs their response, the answer is stored in variable @ans

below this text is an example of what it looks like.
```
<img width="351" height="90" alt="image" src="https://github.com/user-attachments/assets/6c490373-8b14-4882-9321-7e1a111cdb33" />

```# everything here is NOT final and subject to change
# the var command (assignment to variables)
var [str] @myStrVar "Content should be in this string"
var [int] @myIntVar 32 # the 32 part can be a string and still work if its a valid convertible number:
var [int] @myIntVar "32"

# note: this will most definitely stay like this but its here just incase.
cls # clearscreen command. Wow, so awesome.

# now here is the most awesome command here
ex "echo hi"
# the ex command executes a command prompt command, using os.system()
```
Now since I've shown all the stuff, let me show you an example script

```io term in "What is the capital of France? (Case sensitive) > " @ans
if @ans == "Paris" {
io term out "Correct!" [l]
} e {
io term out "Sorry... incorrect." [e]
}
```
