
# Problem Statement for Project-1-RJP
For a medium sized fleet of a grounds maintenance company there is a robust methodology in use for creating a fuel use projection for the coming year.  However tyre costs fluctuate and previous budget projections have been inaccurate.  

“Can we use clustering to provide a model of a relationship between fuel costs and tyre costs for the previous year, which could be used to improve the budget projection for future tyre costs?”

For this exercise solely focus on fuel cost and tyre cost relationship.

For future exercises it would be possible to include other variables such as:

•	Total miles driven 

•	Driver speeding and safety scores

•	Historic weather conditions

# Summary
To address the problem statement we worked in GitHub to collaborate on the same data.

Ruth Havis supplied raw data for 2018 fuel costs by vehicle ergistration in litres of fuel and 2018 tyre sepnd in £ by vehicle registraation. Jack Kennison converted this to a useable csv format.  Initial R code written by Jack Kennison was used to plot and model the 2 variables using K Clustering, however the model was not very useable in the first iteration. 

Priya Shah worked on the data using manual K Clustering to see if the results were different, which they were.  She also grouped the vehicles by year of manufacture which provided a possible model and useful information on one vehicle with an outlying fuel spend.  This can be seen in our submitted files.

Ruth continued the work with Jack's code, adding scaling to the variables at Peter Jones' suggestion. This gave a much more useable model because one variable (fuel spend) was far larger than the other which had previously been skewing the results.  Scaling provided a more useful result and viable clusters.  

Jack then used the Knit to PDF function from the Tidyverse library and MikTex to enable the output to be stored and sent as a PDF.
This, along with the GitHub repository forms our submitted project.

# Conclusion
In conclusion the model of K Clustering shows there is likely to be a relationship between fuel spend and tyre spend during a year.  However it is also a reasonable conclusion that a further factor is needed to give a viable model for budgeting (for example vehicle make and model).  The modelling shows there is likely to be some outliers which may need investigation and possibly removing from the data in order to develop a robust model for budgeting.  But overall the project has shown it should be possible, using data analysis, to build a better prediction of annual tyre costs.
