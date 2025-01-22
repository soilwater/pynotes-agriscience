# Coding Guidelines

The steps below are aimed at new coders to help them indetify the purpose of the code, stimulate the process of breaking down problems into smaller pieces, and logically organize these smaller components or steps. Writing clean and human-readable code requires consistency and the adoption of good programming practices and habits.

### Define the goal of your code
Briefly describe the purpose of the code. What do you want the code to do? Here it is important to be as specific as possible.

### Create a sketch to break down the problem
To decompose the problem into smaller steps it is a good idea to sketch the components and flow of your tentative code. Iterative sketching and drafting will help you clarify your ideas. Start by describing the source of input data and the intended output of your code. If your code relies on multiple equations, filters, or intermediate computations, add them to the sketch so that you can gradually build the logic of your code.


::: {.callout-tip}
## Tip

In this step it is important that you consider starting from scratch all over again if necessary. Sometimes we get entangled with our own ideas and a fresh start can be the best solution.
:::


### Adopt version control
Whether you are a solo coder or part of a team, adopting version control tools (e.g. Git, GitHub) is a must in modern science to keep track of changes and backup your code. Although not ideal, even tools like Dropbox and OneDrive will be a step forward, and may allow inexperienced coders that feel intimidated by more advanced tools to remain engaged with good coding practices.


### Draft the code
This is the part were we write and test the code for the first time. Below is a list of good coding habits that you may want to consider during this process:

* At the top of you code, include your name, date, a brief description of the purpose of the code, and, if necessary, provide the reference to a manuscript, book, or blog.

* Code one or a few lines at the time. 

* Before running any code, set an expectation for the output. Whether you are running a simple `print` statement or several lines of code, ensuring that you are obtaining the desired outcome will prevent that errors accumulate and propagate in your code.

* Use cells in Jupyter notebooks to break down the problem into smaller pieces. Write and test the code for each cell before proceeding to the next part of the problem.

* Add one to three sentences at the beginning of any function or script describing the purpose of the code (in functions this is called the *docstring*).

* If you follow the steps or equations detailed in a peer-reviewed manuscript or book, add a comment next to each line referencing the equation number or page number.

* When defining inputs, outputs, and the intermediate variables add a comment with the units.

* Use descriptive variable names. Err on the verbose side instead of assigning cryptic variable names. Exceptions may apply when coding equations from a specific source.

* Write descriptive variable names using underscores (e.g. air_temperature)

* Function names should be all lower case with no underscores (e.g. thermaltime()).

* Use spaces to improve readability, but avoid extraneous whitespace inside parentheses, brackets, and braces. For instance: `c = (a+b) * (a-b)` is better than `c = (a + b) * (a - b)`.

* If a block of code is long and complicated, consider splitting the code into smaller blocks. If this is not possible, use white space and meaningful comments to explain the steps of the code. 

::: {.callout-note}
## Note
I highly encourage you to check the [Python style guide](https://peps.python.org/pep-0008) for detailed guidelines and examples:
:::

### Error debugging
Encountering errors and making mistakes is a natural part of the coding process. Rather than expecting perfection at every step, embrace these moments as critical learning opportunities. I recommend writing a line of code, then testing it to ensure it behaves as expected before moving on. Always have a clear expectation for each line's output - this approach not only helps in identifying errors early but also deepens your understanding of how your code functions.

::: {.callout-tip}
## Tip
A frequent pitfall among new programmers is assuming that a line of code is correct without thoroughly testing or questioning the logical validity of its output. Always approach code with a clear expectation of the outcome.
:::

One of the more frustrating aspects of coding is how small syntax errors, like a missing parenthesis, an extra comma, or a misspelled function name, can stop your code from running entirely. When you're new to coding, these details can be easily overlooked. Almost every coder can recall a time they spent an entire afternoon troubleshooting a simple typo. Therefore, it's crucial to meticulously examine your code to ensure everything is correct and functioning as intended.

### Code review
Ensure that others read your code. Don't take criticism personally. If something is not clear it might be due to bad syntax, improper logic, or lack of documentation. If you are the reviewer, be respectful, honest, and provide constructive feedback.

### Refactor code
This step is about polishing the code by implementing one or more of the following: adding comments, renaming variables with more meaningful names, merging cells with related code for a more compact code, re-writing lines of code in a more time-efficient way, replacing code with more modular functions, removing unnecessary code, replacing loops by element-wise operations, pre-allocating memory, etc. 


## References

Van Rossum, G., Warsaw, B. and Coghlan, N., 2001. PEP 8: style guide for Python code. Python. org, 1565. The official Python style guide (PEP 8) can be found [here](https://www.python.org/dev/peps/pep-0008/). 