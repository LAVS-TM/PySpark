# PySpark [![Profile][title-img]][profile]

[title-img]:https://img.shields.io/badge/-LAVS-blue
[profile]:https://github.com/LAVS-TM

### Root

* `project_part1.ipynb` is our first part with the data analysis and with the insights of the stocks.
* `project_part2.ipynb` contains the part 2 of the project with the machine learning on the data.
* `data` contains the data of the project.
* `Big_Data_presentation.pdf` is our slides for the final presentation.




RAND is a repository for a sport **dataset analysis** made with the language **R**. The analysis is done in `Projet_final_Lemonnier_Alexandre_Simonin_Victor.ipynb` with a dataset description, some **statistical analysis**, **visualisation**, a **PCA** (Principal Component Analysis ) and finally a **logistic regression**.


## Dataset

The dataset is here in `/data/decathlon.csv`. The dataset is made up of several quite different pieces of data. These represent the scores obtained by athletes in the **decathlon** event at the **Olympic Games** and at the **Decastar**, we have the scores of the 10 events as well as their ranking and their points.

<img src="https://github.com/LAVS-TM/RAND/blob/main/readme_images/dataset.png" alt="Dataset">


## PCA

We perform a **PCA** (Principal Component Analysis) in the notebook.

This allows us to analyze and visualize our Decathlon dataset, which contains individuals described by several quantitative variables.

**PCA** is a method that allows us to explore data with multiple variables. Each variable could be considered as a different **dimension**. This is useful because it could be very difficult to visualize our data in a **multidimensional** "hyper-space".

## Correlation

We also visualize our data with a **correlation graph** :

<img src="https://github.com/LAVS-TM/RAND/blob/main/readme_images/corr.png" alt="Correlation">

We made few analysis on it:

- The results of the short race events, therefore `100m`, `400m` and `110m.H`, are strongly correlated with each other. Quite surprisingly, however, they are negatively correlated with the final ranking, unlike the `Length`, `Weight` and `Height` events.
- The `Length` event and the `400m` event are quite strongly negatively correlated.

## Representation

Finally there is a representation on the **factorial axis** that allows us to notice the quality of representation of our variables.
Here, the axes must be interpreted **independently**.

<img src="https://github.com/LAVS-TM/RAND/blob/main/readme_images/factorial.png" alt="Factorial Representation">

Several elements can be analysed:

* **Positively** correlated variables are grouped together.
* **Negatively** correlated variables are positioned on opposite sides of the origin of the graph (opposing quadrants).
* The distance between the variables and the origin measures the **quality of representation** of the variables. Variables that are far from the origin are well represented by **PCA**. For example, the throwing events, namely `Shot Put`, `Discus` and `Javelin`, are strongly correlated because they point in the same direction. However, `Javelin` is less well represented than `Weights` and `Discs` in the first two **principal components**.