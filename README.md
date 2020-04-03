# Introduction
In this project, we will be using 3 cluster analysis in order to investigate what are the most common jobs post-college for JHU graduates. We will begin the Analysis by finding the 3 departments that are most representative of their cluster by minimizing their z scores. The z scores we're most interested in will be the number and the percentage of students in each major that go into the fields of Academia, For Profit, Goverment work, and the students that are left untracked. From this investigation, we arrive at the following 3 clusters with a minimized distance sum of 108.75 
</br>
# Analysis
In order to determine our clusters and do a cluster analysis, we began by the mean and sigma of each major's:
</br>
-Number of students that went into the fields of Academia, For Profit, Non Profit, Goverment work, and N/A </br>
-Percentage of students that went into the fields of Academia, For Profit, Non Profit, Goverment work, and N/A </br>
The mean and sigma were founding using the AVERAGE and STDEV tools. </br>
Next, we found the z score of each major by using the STANDARDIZE tool for each column. Using these z scores, we then found the distance between each row of z scores and the row of z scores from an arbitrary cluster using SUMXMY2. </br>
This process was repeated for 3 arbitrary clusters and the minimized z-score was then summed to give the Summed Distance which we aim to minimize. Using Solver, we minimized the Summed Distance, set the departments as moving variables, and then proceeded to find the clusters that were most representative of the multivariable midpoints of our data. </br>

![Alt Text](https://github.com/danielhong3/ClusterAnalysisOfJHUGraduatesRightOutOfCollege/blob/master/ClusterFinal.JPG)

From this final result, we can tell that: </br>
-Cluster 1 was centered around Pharmacology, and this cluster favored primarily For-Profit </br>
-Cluster 2 was centered around Clinical Investigation, and this cluster was centered around N/A. Indicating that departments that fall around this cluser do not have sufficient data surrounding them to indicate much about this students right after college. </br>
-Cluster 3 was centered around Biochemistry, Cellular, and this cluster favored Academia. Unfortunately, this cluser also favored N/A fairly heavily, indicating that departments centered around this cluser may also not have sufficient data to say much about thier students after college. </br>

#References:
https://provost.jhu.edu/wp-content/uploads/sites/4/2019/02/Career-Outcome-ADA-Tables-Final.pdf
