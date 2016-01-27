## Livedemo ?

## Topics to include:
* auto-completion and auto-indentation out of the box (it's possible to do this in standard python REPL, but it requires quite some work: http://conjurecode.com/enable-auto-complete-in-python-interpreter/)
* command? command??
* %cpaste / %paste
* %edit - allows you to open your favorite editor, white a multi-line command there and execute that code. %edit -p allows you to reopen the editor with last command (useful if you have made a typo)
* using IPython for debugging: using ipython.embed() in your code or using %debug in IPython
* ipython notebooks (+ project jupiter)

### Topics to maybe include:
* ipythonrc (aliases ?) (vs https://docs.python.org/2/using/cmdline.html#envvar-PYTHONSTARTUP)
* prompt tuning (http://ipython.org/ipython-doc/rel-0.10.2/html/config/customization.html) ?


## Other interesting features:
* IPython has String lists - they are used to process output from system commands (they are produced when you run var = !cmd). You have some special commands to convert those lists to a string or path objects (for file manipulation) ([source](https://ipython.org/ipython-doc/3/interactive/shell.html), [examples on slide 8](https://speakerdeck.com/zsiciarz/ipython-tips-tricks-magic))
* You can easily repeat steps from the history by calling %history 6-8 (it will repeat commands 6,7,8) ([source or slide 11 ](https://speakerdeck.com/zsiciarz/ipython-tips-tricks-magic))
* Session logging: you can log your IPython sessions to a file and then resume it from the file log
* One-line timing: %timeit (line mode) or %%timeit (cell mode)
* %pastebin - instant code snippets on gist.github that you can share with someone
* %macro - creates a macro (set of commands) from the commands you have previously executed, for example %macro test 1-2 5 7-10 will create a macro that will run commands from line 1,2,5,7,8,9,10 ([source](http://pages.physics.cornell.edu/~myers/teaching/ComputationalMethods/python/ipython.html)
* You can combine stuff, for example, create a macro with %macro and then edit it with %edit