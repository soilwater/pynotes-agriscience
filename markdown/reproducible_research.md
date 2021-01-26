# Reproducible Research

The idea behind reproducible research is to support published studies with datasets of field or lab observations, model outputs, instrument data, and the code use in data analysis so that others can reproduce the same findings.

Perhaps, the best advantage of using a high-level programming language is the ability to load data in a standard and cross-platform format (e.g. .txt, .csv), then conduct numerical, statistical, and geographic analyses, and generate publication-quality figures, all within the same environment. In other words, the goal is to concetrate the steps of data analysis in a single platform using code to document our reasoning and logic, minimizing or completely eliminating the need ofs multiple specialized softwares.

>Think about how many mouse clicks and keyboard strokes you have to repeat to re-run the entire data analysis for a manuscript when using several softwares.

By writing code within a single platform we create step-by-step and logically arranged machine-executable instructions that enable us to reproduce our data analysis from top to bottom at anytime. The detailed sequence of steps also allows other people to follow our reasoning, reproduce our findings, and check our work (e.g. manuscript reviewers, graduate advisors).

Here are my top three reproducible research practices for research:

1. Avoid manipulation of raw data. This includes files collected by dataloggers, data retrieved from online sources, or field/lab spredsheets. If you are copy-pasting data, you are probably doing it wrong.

2. Document and structure your code so that is human-readable. This step requires adding comment lines, making use of white space (or cells) to breakdown the code into smaller sections, add equations with reference to books and manuals, and embed figures. 

3. Provide public access of observations, data, and code through:

    - dedicated version-control platforms for creating and sharing code like Github and Gitlab. 
    - use a general-purpose open-access repository like Zenodo, which also generate a digital object identifier (DOI)
    - even tools like Dropbox and OneDrive are a step forward for making your research findings reproducible. 
    - host the entire content in your own research website.


## Jupyter Notebooks

A Jupyter notebook is a web-based environment for interactive computing. Jupyter notebooks seamlessly aggregate executable code, code documentation, equations, figures, images, and paths or URL links to specific datasets within a single platform.

- Code lives in cells, which help organizing your code. The main advantage of cells is that you can run (i.e. execute code) cells individually to ensure that the code is working properly before you move forward.

- To run code in a cell press: `ctrl + enter` keys. The result will appear right below the code.

- To run code in a cell and move onto the next cell when done press: `ctrl + shift + enter` keys

<br/>

![alt_text](../media/jupyter_lab_gui.png "Jupyter Lab GUI")
*Mac users can use double tap with two fingers for zooming the image*



## References and recommended reading

[Guo, P., 2013. Helping scientists, engineers to work up to 100 times faster.](https://dl.acm.org/doi/10.1145/2507771.2507775)

[Shen, H., 2014. Interactive notebooks: Sharing the code. Nature, 515(7525), pp.151-152.](https://www.nature.com/news/interactive-notebooks-sharing-the-code-1.16261)

Sandve, G.K., Nekrutenko, A., Taylor, J. and Hovig, E., 2013. Ten simple rules for reproducible computational research. PLoS computational biology, 9(10).

Skaggs, T.H., Young, M.H. and Vrugt, J.A., 2015. Reproducible research in vadose zone sciences. Vadose Zone Journal, 14(10).