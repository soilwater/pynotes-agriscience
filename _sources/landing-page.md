# PyNotes for Agriscientists

A set of hands-on coding exercises to solve common tasks and simple problems in agricultural sciences.

<a href="https://zenodo.org/badge/latestdoi/181793782"><img src="https://zenodo.org/badge/181793782.svg" alt="DOI"><a>


## Audience

This material is part of an introductory graduate level course offered to students in plant and soil sciences with little or no programming experience. However, anyone with sufficient discipline to follow along the notes and interested in learning how to code, become more productive, and embrace reproducible research practices should (hopefully) find the content of this notes useful. The material is aimed at students that are transitioning from spreadsheets analysis to a programming environemnt and that first need to learn basic building blocks before tackling more complicated challenges. Most examples and datasets are in tabular format, so that you can open the files with your favorite spreadsheet software and inspect the data and compare your solutions.

The Python language was selected because it is free, has a relatively straightforard and simple syntax, has been widely adopted by the scientific community, and contains a rich ecosystem of libraries and tools for generating reproducible research (e.g. Jupyter Notebooks). 

These notes are intended to be simple and explicit, and code expressions may not be the most efficient or *pythonic*. As students acquire more experience through the different exercises, they will become more familiar with the syntax, documentation sources, and eventually will be able to write more advanced and elegant code. 


## Motivation

These notes stem from the need to increase code literacy in students pursuing a career in agricultural sciences. With the increasing volume of data used in agricultural production and the need for new and reproducible ways to analyze these data beyond traditional spreadsheets, scientific programming is becoming an essential skill for agriscientists.

The three main aspects that motivated this material are:

1. The lack of online examples including real datasets in environmental sciences. The material presented in this series of Jupyter notebooks relies entirely on data from published studies in peer-reviwed journals or data collected by the author and his students as part of research projects;

2. The vast amount of existing material about coding is either aimed at the general public with trivial examples or learners familiar with advanced concepts in computer science, both of which have little appeal to graduate students and early career scientists in environmental sciences that are learning to write code for the first time.

3. I wanted to create a set of short, interactive, and reproducible scripts in the form of notebooks that students can download and execute anytime. Students can take advantage of tools such as [Github](https://github.com) and [Binder](https://mybinder.org) to gain access to the entire material and start coding in a matter of minutes.


## Goals

Students who successfully complete the material should be able to:

- construct effective, well-documented, and error free scripts and functions.
- apply high-level programming to generate publication quality figures and optimize simple models.
- find information independently for self-teaching and problem solving.
- learn good programming habits and basic reproducible research practices by following short exercises using real data.

    
## Datasets

The datasets used along these notebooks can be found in the `/datasets` directory of the Github repository. Throughout the examples it is assumed that the Python interpreter of the Jupyter notebook is in the `pynotes/notebooks` directory, reason why the directories are relative to this path in the exercises, for example: `pd.read_csv("../datasets/file.csv")`. 

If you want to follow along an exercise without downloading the entire material, you can always read the data directly from the Github repository, just make sure you get the "Raw" URL link. For example, to read the Anscombe's dataset:

`pd.read_csv('https://raw.githubusercontent.com/andres-patrignani/pynotes/master/datasets/anscombe_quartet.csv')`

Follow this video to learn how to obtain the link for the raw data.


![](media/read_dataset_from_github.gif)


## About the author

Andres Patrignani is an Assistant Professor in Soil Water Processes in the Department of Agronomy at Kansas State University. You can contact me at `andrespatrignani@ksu.edu`


## Feedback

All the code has been written with teaching in mind. If you spot an important error or a *big no-no* that should not be taught to students, please share your opinion and suggestions.
    
- For bug reports, code suggestions, and topic requests please open an issue in the [Github repository](https://github.com/andres-patrignani/pynotes/issues).

- For other related issues feel free to contact me at andrespatrignani@ksu.edu


## Support

The content of this website is used as a foundation for a gradaute level course in Scientific Programming and Reproducible Research offered every Spring semester in the Department of Agronomy at Kansas State University.

This initiative is partially supported by the Kansas State University [Open/Alternative Textbook Initiative](https://www.lib.k-state.edu/open-textbook)


## License

All the code in these Jupyter notebooks has been written entirely by the author unless noted otherwise. The entire material is available for free under the Creative Commons Attribution-NonCommercial-ShareAlike ([CC BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/)) license
