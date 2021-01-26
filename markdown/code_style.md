# Coding Style

Writing clean, easy-to-read, and correct code requires consistency and the adoption of good programming habits. Sometimes emphasis is placed on writing code within teams, but the code should be clean and well-organized even if you are the only user. 

In this section my goal is to suggest some coding habits (within the scientific environment) and guidelines.


## Good coding habits

* Use cell mode (e.g. Jupyter notebooks, Matlab Live Script) to break down the problem, and build and test your code step by step. Proceed to the next step only after the current cell is producing the desired outcome.

* Add one to three sentences at the beginning of any function or script describing the purpose of the code. Provide references to websites, books, or research manuscripts.

* Use descriptive variable names. Exceptions may apply when coding equations from a specific source. In that case, document the page number and/or equation number as a comment next to each line of code.

## Python syntax

* Write descriptive variable names using underscores (e.g. air_temperature) or camel case (e.g. airTemperature). Adopt one or the other and be consistent throughout the code.

* Constants and matrices are usually denoted using upper case letters (e.g. PI, LAMBDA).

* Function names should be all lower case with no underscores (e.g. thermaltime()).

* Module names should be all lower case.

* Add a space before and after equal, plus, and minus signs to improve readability (e.g. a = 2 + 3).

* Add units as a comment when defining constants, input variables, and output variables.

## References

Van Rossum, G., Warsaw, B. and Coghlan, N., 2001. PEP 8: style guide for Python code. Python. org, 1565. The official Python style guide (PEP 8) can be found [here](https://www.python.org/dev/peps/pep-0008/). 