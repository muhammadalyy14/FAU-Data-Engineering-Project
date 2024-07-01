# Exercise Badges

![](https://byob.yarr.is/muhammadalyy14/FAU-Data-Engineering-Project/score_ex1) ![](https://byob.yarr.is/muhammadalyy14/FAU-Data-Engineering-Project/score_ex2) ![](https://byob.yarr.is/muhammadalyy14/FAU-Data-Engineering-Project/score_ex3) ![](https://byob.yarr.is/muhammadalyy14/FAU-Data-Engineering-Project/score_ex4) ![](https://byob.yarr.is/muhammadalyy14/FAU-Data-Engineering-Project/score_ex5)

# Climate Disaster Trends and Risk Correlation Analysis

The project will leverage two comprehensive datasets to explore the above questions. The datasets include information on the frequency of climate-related disasters and climate-driven INFORM risk indicators. By integrating and analyzing these datasets, the project aims to provide insights into the global trends of climate-related disasters, identify the most affected regions, and evaluate the correlation between disaster severity and risk indicators.

# Datasources

<!-- Describe each datasources you plan to use in a section. Use the prefic "DatasourceX" where X is the id of the datasource. -->

# Datasource # 1: Climate-related Disasters Frequency
* Data URL: https://opendata.arcgis.com/datasets/b13b69ee0dde43a99c811f592af4e821_0.csv
* Metadata URL: https://climatedata.imf.org/datasets/b13b69ee0dde43a99c811f592af4e821_0/about
* Data Type: .csv

This dataset, sourced from EM-DAT by the Université catholique de Louvain, tracks the frequency of various climate-related disasters globally from 1980 to 2022. It includes detailed records for different types of disasters such as droughts, floods, extreme temperatures, landslides, storms, and wildfires. Each entry specifies the country affected, the type of disaster, and the annual occurrence data. This dataset enables an analysis of trends over decades to understand how the frequency of these disasters has changed in response to global climate change.

# Datasource 2: Climate-driven INFORM Risk
* Data URL: https://opendata.arcgis.com/datasets/7cae02f84ed547fbbd6210d90da19879_0.csv
* Metadata URL: https://climatedata.imf.org/datasets/7cae02f84ed547fbbd6210d90da19879_0/about
* Data Type: .csv

The Climate-driven INFORM Risk Indicator, adjusted annually by IMF staff, provides a comprehensive assessment of the risk associated with climate-driven hazards. It focuses on three dimensions: hazard & exposure, vulnerability, and lack of coping capacity. Each country's data from 2013 to 2022 reflects the aggregated risk posed by potential climate-related events such as floods, tropical cyclones, and droughts. This dataset aids in evaluating the preparedness and vulnerability of different nations to handle climate-induced disasters.

## Project Work
Your data engineering project will run alongside lectures during the semester. We will ask you to regularly submit project work as milestones so you can reasonably pace your work. All project work submissions **must** be placed in the `project` folder.

### Exporting a Jupyter Notebook
Jupyter Notebooks can be exported using `nbconvert` (`pip install nbconvert`). For example, to export the example notebook to html: `jupyter nbconvert --to html examples/final-report-example.ipynb --embed-images --output final-report.html`


## Exercises
During the semester you will need to complete exercises using [Jayvee](https://github.com/jvalue/jayvee). You **must** place your submission in the `exercises` folder in your repository and name them according to their number from one to five: `exercise<number from 1-5>.jv`.

In regular intervalls, exercises will be given as homework to complete during the semester. Details and deadlines will be discussed in the lecture, also see the [course schedule](https://made.uni1.de/). At the end of the semester, you will therefore have the following files in your repository:

1. `./exercises/exercise1.jv`
2. `./exercises/exercise2.jv`
3. `./exercises/exercise3.jv`
4. `./exercises/exercise4.jv`
5. `./exercises/exercise5.jv`

### Exercise Feedback
We provide automated exercise feedback using a GitHub action (that is defined in `.github/workflows/exercise-feedback.yml`). 

To view your exercise feedback, navigate to Actions -> Exercise Feedback in your repository.

The exercise feedback is executed whenever you make a change in files in the `exercise` folder and push your local changes to the repository on GitHub. To see the feedback, open the latest GitHub Action run, open the `exercise-feedback` job and `Exercise Feedback` step. You should see command line output that contains output like this:

```sh
Found exercises/exercise1.jv, executing model...
Found output file airports.sqlite, grading...
Grading Exercise 1
	Overall points 17 of 17
	---
	By category:
		Shape: 4 of 4
		Types: 13 of 13
```
