# Coding Guidelines

The steps below are aimed at new coders to help them indetify the purpose of the code, stimulate the process of breaking down problems into smaller pieces, and logically organize these smaller components or steps.

## Define the goal of your code
Briefly describe the purpose of the code. What do you want the code to do? Here it's important to be specific.

## Break down the problem (Sketch + pseudocode)
It's time to put the pieces of the puzzle together. To break down the problem into smaller steps it is always a good idea to sketch the flow and components of your code on a whiteboard or a piece of paper. Use a canvas that you can erase. At this point you may not know exactly all the steps and complications of your code. Iterative sketching and drafting will clarify your ideas. It's this iterative process that will provide you with alternative ideas, new insights, and tentative decisional points that will control the flow of your code. If your code relies on multiple equations, add them to the sketch so that you can build the logical flow of your code.

Describe whether inputs will be retrieved from a remote server, the file system, or from the the user through an interactive interface. Identify potential functions that may emerge from this work and that can be re-used throughout the code.

>In this step is important that you consider starting from scratch all over again if necessary. Sometimes we get entangled with our own ideas and a fresh start can be the best solution.

Another effective technique to clarify your ideas is to literally breakdown the problem into smaller steps using your own words either below the sketch or at soem specific points of the flow chart.

## Adopt version control
To keep track of changes and backup your code it is an imperative practice in modern science to adopt version control tools (e.g. git), whether you are part of a team or if you are working alone. Although maybe not ideal, even tools like Dropbox and OneDrive will be a step forward and may allow inexperienced coders that feel intimidated by more advanced tools to remain engaged.

## Draft the code
In this step it is important that you adopt good programming habits. Always include your name, date, purpose of the code, and a brief description of inputs and outputs (units, data type, mandatory/optional inputs). Make sure you include meaningful comments.

If a block of code is long and complicated, consider splitting the code into a more amenable length. If this is not possible, then take your time to add some comments every so and then to explain in more detail the purpose and steps of the lengthy code. 

If you follow the steps or equations detailed in a peer-reviewed manuscript, add a comment next to each line referencing the equation number and page number. Provide the full reference either at the beginning or end of the code.

## Error debugging
Finding the errors in your code is critical. This will not happen at a particular point. We make mistakes all the time while coding. So I encourage you to write a line of code and then test your code before you proceed. Do not proceed until the line of code you are writing does what you expect it to do. It's important that before running each line of code you should have an expectation for the output.

>One of the greatest pitfalls from noice coders is assuming that a line of code is returning the correct output without testing, or testing without questioning whether the output makes logical sense.

An extremely annoying thing about writing code is that seemingly irrelvant syntax errors will prevent the code from running from beginning to end. A missing parenthesis, a missing dot, an extra comma, or misspelling a function name will likely result in an error. When you are starting to code, many of these nuances are invisible. I guess every coder has a story on how they wasted an entire afternoon because of a typo. 

Meticulous examination of your code is mandatory to ensure correctness. Using pseudocode, you can debug your code using the following reasoning:

```python
    Run code
        while number of errors > 0
            Find error
            Fix error
    end
```

## Code review
Ensure that others read your code. Don't take criticism personally. If something is not clear it might be due to bad syntax, improper logic, or lack of documentation. If you are the reviewer, be respectful, honest, and provide constructive feedback.

## Refactor code
This step involves improving the time efficiency of the code by re-writing some lines of code in a more time-efficient way, by replacing functions with similar but more efficient (or newer) functions, removing unnecessary code from loops, replacing loops by element-wise or array operations, by pre-allocating memory, etc. 

Also, pay special attention to parts of the code that need changes to meet a specific code style, add meaningful comments, and be sure to have a well-documented help section at the beginning of the code.

Polishing your code is essential to take it to the next step. Test every change to ensure that the code does not change its behavior. Polish your code one or few lines at the time.

<br/><br/><br/>

*Note: These steps have been devised with the help of Tyson Ochsner while teaching a Matlab course in 2015*