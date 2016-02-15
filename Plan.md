* Hello, after a nice presentation from Indico guy about Ipython notebooks, where you have seen some examples of what Ipython can do, I wanted to convince you to ditch the "Python" REPL and switch to IPython in the command line.
* What is IPython ? It's like Python REPL - you type some code, you hit enter and the code get executed (or you get an error). But it's way cooler than Python REPL.
* First, it has tab completion. Awesome.:
    - example of string replacement function
* Then, it has a very easily accessible documentation. You don't remember what a function was doing ? No problem, put function?. You want the whole source code ? Put function??
    - example of sort function - we check the documentation to see if it happens in place or not
* IPython has a bunch of magic functions built-in (no, they are seriously called "magic functions")
* If you want to copy some code chunk, use %cpaste or %paste (check the difference)
* What do you do when you want to quickly write a multiline function ? In Python, you can try, but you need to always remember about appropriate number of indentation and if you realize that you need to put some code above you current line then you are screwed. In IPython, you don't need to worry about the indentation so much and if you need to put some code in the line above then, well you are still screwed. But, magic to the rescue. In situations like that you can use %edit function - it will open your favourite editor (or Vim, if you always forget to configure $EDITOR variable properly) where you can type your code and after you close it, it will execute this code. **find a nice example of easy function that I can debug and then edit**
* Ups, we have an error. We can debug the error with %debug command.
* Ok, so we know what was wrong - how do we fix it ? Easy, we run %edit with -p option. It will reopen you editor with the last command.
* Go back to the slides and show some more commands:
    - %timeit
    - %pastebin
    - %history
    - %macro
    - %save
* You can execute shell commands by adding `1` at the beginning of the command
* You can also use IPython for debugging: You just drop: ```import ipython; ipython.embed()``` somewhere in the code and then the code execution reaches that place, it will start Ipython session in your terminal.