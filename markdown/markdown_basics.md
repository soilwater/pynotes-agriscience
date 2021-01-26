# Markdown basics

[Markdown](https://www.markdownguide.org/getting-started/) is a simple and minimalist markup language that allows people to focus on writting. One of the nicest features of the Jupyter notebooks is that we can combine code with documentation written in Markdown. This is excellent to provide additional information without cluttering the code with comments and also allow us to pass rich media such as images, videos, and equations. This is why Jupyter notebooks are so great for both teaching and creating reproducible research.

Markdown is a markup language created to speed up formatting without having to write HTML (HyperText markup Language, the language we use to write websites). There is no global standard, and different came up with slightly different variations. The Github-flavored (Kramdown) markdown official documentation can be found here: https://github.github.com/gfm/

The list of example below is only aimed at getting you started. I encourage you to visit the following two links for detailed syntax, cheatsheets, and more comprehensive examples:

- [Excellent syntax guide](https://www.markdownguide.org/basic-syntax/)

- [Adam Pritchard's popular Markdown examples](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

- [John Gruber's original specifications](https://daringfireball.net/projects/markdown/)


## Comments

Markdown does not seem to have an official way of adding comments. However, we can fool several Markdown interpreters by preceding text with the following expression `[//]:`

`[//]: This is a comment`

Note that this trick might not work in some Markdown editors like Typora, but it does work in Github.


## Line breaks
Pressing the `enter` key will not generate empty lines. Because Markdown eventually is converted into HTML, we can use HTML tags to expand the editing and styling possibilities in our document. So, to add a line break, we can use the self-closing line break tag: `<br/>`. 

```
some text
</br>
more text
```



## Headers

Represented by adding 1 to 6 leading `#` signs

```none
# Title header
## Sub-title header
### Sub-sub-title header
```

## Sub-title header
### Sub-sub-title header



## Emphasis

```
*italic text*
_italic text_
**bold text**
__bold text__
~~striked text~~
```



*italic text*

_italic text_

**bold text**

__bold text__

~~text~~




## Highlighting
```none
To calculate the `sin(90)` first import the `math` module`
```

To calculate the `sin(90)` first import the `math` module`


## Monospace font
    Indent text using the Tab key to generate a monospace font.

## Inline equations

```none
$y = ax+b$
```



$y = ax+b$


## Block equations

Example equation for calculating actual vapor pressure (Eq. 17, FAO-56):

```none
$$ea = \frac{eTmin\frac{RHmax}{100}+eTmax\frac{RHmin}{100}}{2}$$ 
```



$$ea = \frac{eTmin\frac{RHmax}{100}+eTmax\frac{RHmin}{100}}{2}​$$ 


    ea = actual vapor pressure (kPa)
    
    eTmax = saturation vapor pressure at temp Tmax (kPa)
    
    eTmin = saturation vapor pressure at temp Tmin (kPa)
    
    RHmax = maximum relative humidity (%)
    
    RHmin = minimum relative humidity (%)

## Block quotes

Use the `>` character to generate block quotes.

```none
>"The programmers of tomorrow are the wizards of the future. You're going to look like you have magic powers compared to everybody else." *- Gabe Newell*
```

> "The programmers of tomorrow are the wizards of the future. You're going to look like you have magic powers compared to everybody else." *- Gabe Newell*

## Bullet lists
Any of these two alternatives:
```none
- item 1    * item 1
- item 2    * item 2
- item 3    * item 3
```

will generate something similar to this:
- item 1
- item 2
- item 3


## Numbered Lists

```none
1. item 1
2. item 2
3. item 3
```
1. item 1
2. item 2
3. item 3


## In-line links
```none
[Github-flavored markdown(https://www.wikiwand.com/en/Home_page)
```



[Github-flavored markdown](https://www.wikiwand.com/en/Home_page)

## Referenced links

```none
[Try a live Markdown editor in your browser][1]

Some text
Some more text

[1] https://stackedit.io "Optional title to identify your source"
```



[Try a live Markdown editor in your browser][1]

[1]: https://stackedit.io	" Stackedit browser Markdown editor"


## Figures

Figures can be inserted in Markdown following this syntax:

```none
![alt_text](https://path_to_my_image/image.jpg "My image")
```


Because we many times want to deploy our Markdown in Github, then using pure HTML is the best option:
```none
<img src="upload.wikimedia.org/wikipedia/en/8/80/Wikipedia-logo-v2.svg" alt="wikipedia_logo" width="100"/>
```

<img src="https://upload.wikimedia.org/wikipedia/en/8/80/Wikipedia-logo-v2.svg" alt="Soil cracks" width="100"/>


## Horizontal lines

You can use three consecutive dashes, astericks, or underscores in this fashion:

```none
---
***
___
```

For instance, typing `---`, we obtain the following line:

---



## Code

We can write inline or block code. Inline code:

```none
`s = "Python inline code syntax highlighting"`
```



`s = "Python inline code syntax highlighting"`

and block code:

```none
​```python
# Creating a matrix or 2D array
M = [[1, 4, 5],
    [-5, 8, 9]]
print(M)
​```
```

```python
# Creating a matrix or 2D array
M = [[1, 4, 5],
    [-5, 8, 9]]
print(M)
```



## Tables

Simple tables are easy to write in Markdown. However, adding more than a handful of rows and/or columns can turn out to be a pain. So, if you want to display many lines I suggest using a Markdown table generator. Some Markdown editors have shortcuts and table generators and there are websites exclusively dedicated to generate Markdown tables. Below I show a trivial example:

```none 
| Textural class  | Sand (%) | Clay (%) |
|:----------------|:--------:|:--------:|
| Silty clay loam | 10       | 35       |
| Sandy loam      | 60       | 15       |
| Clay loam       | 35       | 35       |
```
The leftmost column is left-aligned `:---`, the center column is center-aligned `:---:`, and the righmost column is right-aligned `---:`. The `|` characters don't need to be aligned in order for the Mardown interpreter to properly render the table, but it certainly helps while constructing the table by hand.

| Textural class  | Sand (%) | Clay (%) |
|:----------------|:--------:|:--------:|
| Silty clay loam | 10       | 35       |
| Sandy loam      | 60       | 15       |
| Clay loam       | 35       | 35       |