
# Problem Statement for Project-1-RJP
For a medium sized fleet of a grounds maintenance company there is a robust methodology in use for creating a fuel use projection for the coming year. However tyre costs fluctuate and previous budget projections have been inaccurate.

“Can we use clustering to make any predcitions or find any unexpected relationships between fuel costs and tyre costs for the previous year, which could be used to improve the budget projection for future tyre costs?”

For this exercise solely focus on fuel cost and tyre cost relationship.
For future exercises it would be possible to include other variables such as:
• Total miles driven
• Driver speeding and safety scores
• Historic weather conditions


# Summary
To address the problem statement we worked in GitHub to collaborate on the same data.

# Data Collection
Ruth Havis supplied raw data for 2018 fuel costs by vehicle registration in litres of fuel and 2018 tyre spend in £ by vehicle registration. To obtain the data fuel card downloads month by month were done, then the data was totalled by registration number in excel in litres.  Any invalid registration numbers (i.e. not 7 digits) were removed and the data cleaned up to remove sold vehicles and vehicles where a full year of data was not available.  For tyre data monthly invoices from the tyre supplier were totalled by registration number.  Again the data was cleaned up to remove no vehicle tyres (e.g. for trailers) and sold vehicles.  There was still considerable data left to base the project on.  Collecting and cleaning up the data took around 4 hours. 

# Work completed on the data

Jack Kennison converted the data to a useable csv format. Initial R code written by Jack Kennison was used to plot and model the 2 variables using K Clustering, however the model was not very useable in the first iteration.

Priya Shah worked on the data using manual K Clustering to see if the results were different, which they were. She also grouped the vehicles by year of manufacture which provided a possible model and useful information on one vehicle with an outlying fuel spend. This can be seen in our submitted files.  

Ruth continued the work with Jack's code, adding scaling to the variables at Peter Jones' suggestion. This gave a much more useable model because one variable (fuel spend) was far larger than the other which had previously been skewing the results. Scaling provided a more useful result and viable clusters.

Jack then used the Knit to PDF function from the Tidyverse library and MikTex to enable the output to be stored and sent as a PDF. This, along with the GitHub repository forms our submitted project.

# Interpretation of Results
The results were very difficult to interpret as they stood.  Whilst some groups did form the results did not support the expected interpretation that great fuel spend would lead to great tyre spend.  In some cases this would occur but the clusters did not show a clear relationship. No unexpected relationships were revealed using K means clustering.  However it did indicate that other factors must be part of this, and that it would be valuable to use K means clustering on a wider data set which involved job role and vehicle model to see if other relationships can be found which can be used to create more informed predictions for budgeting. 

# Conclusion
In conclusion the model of K Clustering shows there is likely to be a relationship between fuel spend and tyre spend during a year. However it is also a reasonable conclusion that a further factor is needed to give a viable method for budgeting (for example vehicle make and model). The modelling shows there is likely to be some outliers which may need investigation and possibly removing from the data in order to develop a robust model for budgeting. But overall the project has shown it should be possible, using data analysis, to build a better prediction of annual tyre costs.
