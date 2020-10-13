## IBM Capstone Project

E-MAIL: dannygarcia193@gmail.com         
Data completed: January, 2020

<a href="https://nbviewer.jupyter.org/github/dannygarcia193/Location_Analysis/blob/master/IBM_Capstone_Project.ipynb"><b>Click here<b/></a> to see jupyter notebook.
  
**Project Name:** Initial Location Analysis For Restaurante La Tierra De Tacos

**Project description:** Hello this is my submission to the IBM captone project assignment--a hypothetical project based on IBM's capstone project guidelines. I should note that this project is completely independent as I came up with the research questions, guidelines, data collection strategy etc. 

In this project I display my research, data preprocessing, as well as analysis skill in making an initial location recommendation based on certain hypothetical guidelines that a business requested. 


### 1. Summary of Project

> Restaurante Los Tacos Del Mar had trouble finding a good location within SF to start their business given the size of SF and large quantity of neighborhoods. In order to find a location that aligns with their business strategy, they came up with five requirements that a neighborhood needed to have: 
1. Contain a population of 5,000 + (increase opportunity of traffic and visibility)
2. Near at least one college and surrounded by at least three other types of schools (partnerships with schools and other organizations, and to provide catering/delivery options)
3. Rent at or below the city's average -$3,000
4. Median income of $50,000 or more (safeguard for tough financial times)
5. With minimal competition (mexican restaraunts) and similar venues (ie. restaraunts) nearby

> With the requirements in place, I retrieved relevant data from the U.S. Census, Data SF, and FourSquare's API with the aims of finding tracts that met the requirements set out by the company. Several cleaning steps were needed after retrieving the data. After some filtering of the data,the original 197 tracts in SF were condensed to 18 that met the first three requirements previously mentioned.

> To filter by the last two requirements, I used the K-Means clustering technique and selected cluster 0 as the best representative of the company's business type. In order to fulfill the fourth requirement, I looked through the dataframe and was able to filter out four tracts that contained Mexican restaurants as one of their common venue categories. The remaining tracts were then mapped along with the schools and colleges in order to select the ones that met the last requirement (see intro for reference). The seven tracts that met the last requirement were then shown to the company as potential tracts for the business to look further into. 


### 2. Conclusion

These seven tracts of interest were found to be affluent with a median income mean of 77,701 dollars, and an average gross rent of 2,229 dollars. In particular, tract 615 stood out with their population size nearly doubling the others (13,864), relatively high median income ($103,451), and proximity to several colleges. Special consideration should be given to this tract.

It should be noted, that these results provide only a direction at which the company can conduct further and more detailed anaylsis of the suggested neighborhood locations. Given the methods used in finding the answer to the business question, I can only conclude that the candidate tracts are potential good locations for the company to look futher into as the requirements outlined in the introduction of this report. Despite the limitations mentioned, this report is still useful for the company as it condenses the number of locations that they have to anaylze.

### 3. Figures

#### Figure 1. Nearby Venues Per Select SF Census Tracts Collected Using FourSquare 
<img src="images/1st_Figure.png?raw=true" width="80%" height="80%"/>

#### Figure 2. 10 Most Common Venue Categories in Select SF Tracts
<img src="images/2nd_Figure.png?raw=true" width="80%" height="80%"/>

#### Figure 3.  Choropleth Map With Markers of Select SF Census Tracts 
<img src="images/Screenshot_85.png?raw=true" width="80%" height="80%"/>

#### Figure 4.  Choropleth Map With Markers for Select SF Census Tracts, School, and Colleges
<img src="images/Screenshot_86.png?raw=true" width="80%" height="80%"/>

