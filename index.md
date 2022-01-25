# Portfolio

## Tableau Dasboard & SQL
---
### A dashboard to summarize the Covid Infections 
[![Run in Tableau Public](https://img.shields.io/badge/tableau-Run_in_Tableau-blue?logo=tableau&logoColor=FDBA18)](https://public.tableau.com/app/profile/duy.nguyen1086/viz/CovidDashboard_16429782005130/Dashboard1)

[![Run in SQL in Github ](https://img.shields.io/badge/github-Run_in_SQL-blue?logo=github&logoColor=FDBA18)](https://github.com/duy7590/SQL_Covid19_Tutorial/blob/main/Covid19_Data%20Exploration_%20SQLQuery.sql)


<div style="text-align: justify">
This is a project for me to practice SQL and Tableau and demonstrate the the basic skills to provide some intelligence out of the raw data.
  
For SQL, I used Microsoft SQL Server Management Studio to create a database based on the Covid Data Excel dowloaded from https://ourworldindata.org/coronavirus
Then I setup different tables and play around with different querries before export the final cleaned dataset and take it as an input to Tableau
  
In Tableau, I made a range of different charts based on the data querried from SQL. (Check it <a href="https://github.com/duy7590/SQL_Covid19_Tutorial/blob/main/Covid19_Data%20Exploration_%20SQLQuery.sql"> here</a> ) 
Later, I designed a simple Dashboard in Tableau which could be view from <a href="https://public.tableau.com/app/profile/duy.nguyen1086/viz/CovidDashboard_16429782005130/Dashboard1"> here</a>: 


</div>

<img src="images/CovidDashboard.png" align="center"/>
<img src="images/MSSQL.png" align="center"/>
---

## Recommender system 
---
### Movies recommender system for group of users (not individual user) with different profiles
[![Run in Google Colab](https://img.shields.io/badge/Colab-Run_in_Google_Colab-blue?logo=Google&logoColor=FDBA18)](https://colab.research.google.com/drive/1_N6R65rL_SYoovv1TYbZ1ODRSliodPDW?usp=sharing)


<div style="text-align: justify">
This is projects done in my "Recommender system" course at University of Tampere. The recommender systems aim at suggesting to users items of potential
interest to them. There are quite different approaches for this task. However, there are 2 basic methods when recommending a new item to user:
  • Similar users - user-based collaborative filtering: Make suggestions based on preferences of similar users 
      - Given a user, identify his/her k most similar users: Cosine similarity, Jaccard similarity
      - Produce recommendations based on the items that are liked by those k users: avg ratings, weighted schemes
  • Similar items - item-based collaborative filtering: Exploit relationships between items
      - Compute similarities between items: Cosine similarity, Jaccard similarity
      - Keep for each item only the k most similar items along with their similarity scores
      - Use similarities to calculate ratings for items with no scores 
  
Recommenders are usually designed to provide recommendations adapted to the preferences of a single user. In many situations the recommended items
are consumed by a group of users. However, in this project, we want to address this issue and bring the Recommender system to another level.

First of all, we run the model with 2 method of Group Recommender system:Average method & Least misery method. The basic idea of these 2 method is to produce a Representative Profile from the the group of different user' profiles.

However, there are weaknesses in both average and least misery methods 
• Average method: the out-flier user is never satisfied
• Least misery method: the system recommends movies not highly interested by anyone in the group

Another important drawback/assumption for the Group recommender based on these 2 method is that:  each time a group is using the recommender system is distinct from the previous ones. This is not a good system.

So, the last step we implemented is using the Sequential Group Recommendations.The idea of Sequential Group Recommendations is: To get a better compromise of getting all group members satisfied enough, and taking into account the opinion of the possible disagreeing member.

For more detail of the implementation, please check the notebook file



</div>

<img src="images/Recommender/1.png" align="center"/>
<img src="images/Recommender/2.png" align="center"/>
<img src="images/Recommender/3.png" align="center"/>
<img src="images/Recommender/4.png" align="center"/>
<img src="images/Recommender/5.png" align="center"/>
<img src="images/Recommender/6.png" align="center"/>
<img src="images/Recommender/7.png" align="center"/>
---

## Data visualization

### Stock & Crypto Portfolio Performance 
[![Run in Google Colab](https://img.shields.io/badge/Colab-Run_in_Google_Colab-blue?logo=Google&logoColor=FDBA18)](https://colab.research.google.com/drive/1D9QBZW4VHcVrJ9rJdX56_YYCNiETPT0e?usp=sharing)

This project has been done based on my real experience with the investment in stock market and crypto market.

During the period of 2018-2019, i have researched about Blockchain technology and learn about its tremendous pontential in the new age of technology. One of the best things about the blockchain is that, because it is a decentralized system that exists between all permitted parties, there’s no need to rely onintermediaries (Middlemen). Apart from its payment feature, the most important usecase of Crypto is smart contracts, otherwise called self-executing contracts, blockchain contracts, or digital contracts. smart contracts not only define the rules and penalties around an agreement in the same way that a traditional contract does, but also automatically enforce those obligations.

Seeing its potential in the future, I decided to invest in a small amount of Ethereum, one of the 2 most popular crypto in the market right now besides Bitcoin.

During the beginning of 2020, due to the Covid pandemic, investor's fear of economic crisis had resulted in a big crash in the global stock market as well in Finland. At this point I considered the stock values in OMX Helsinki Stock Exchange had been significantly undervalued. As a resulted, I decided to investment in 2 top shares in OMX (based on Market Capitalization) which are NOKIA and FORTUM.

This project has been done to visualize the gain and loss of my 3 positions in Crypto (Ethereum) and Stocks (Nokia and Fortum). As well as compare their performance with ther performance of OMX Index during the same period.

My Entry was as below:
<table style="height: 242px;" width="697">
<tbody>
<tr>
<td style="width: 139px;">Acquisition Date</td>
<td style="width: 139px;">&nbsp;Ticker</td>
<td style="width: 139px;">Quantity</td>
<td style="width: 139px;">Unit Cost &euro;&nbsp;</td>
<td style="width: 140px;">&nbsp;Cost Basis &euro;</td>
</tr>
<tr>
<td style="width: 139px;">&nbsp;03/31/20&nbsp;</td>
<td style="width: 139px;">&nbsp;NOKIA.HE</td>
<td style="width: 139px;">1000&nbsp;</td>
<td style="width: 139px;">&nbsp;2.78</td>
<td style="width: 140px;">&nbsp;2780</td>
</tr>
<tr>
<td style="width: 139px;">&nbsp;03/31/20&nbsp;</td>
<td style="width: 139px;">FORTUM.HE&nbsp;</td>
<td style="width: 139px;">&nbsp;100</td>
<td style="width: 139px;">&nbsp;13.4</td>
<td style="width: 140px;">1340</td>
</tr>
<tr>
<td style="width: 139px;">09/16/19&nbsp;</td>
<td style="width: 139px;">&nbsp;ETH-EUR</td>
<td style="width: 139px;">&nbsp;10</td>
<td style="width: 139px;">191.98&nbsp;</td>
<td style="width: 140px;">&nbsp;1919.8</td>
</tr>
</tbody>
</table>
<!-- DivTable.com -->

<img src="images/Portfolio_tracker.png" align="center"/>


---
### GLOBAL SITUATION OF COVID-19
[![Run in Google Colab](https://img.shields.io/badge/Colab-Run_in_Google_Colab-blue?logo=Google&logoColor=FDBA18)](https://colab.research.google.com/drive/1Z9UFhFYL-Eo-G19sHSMm2-wYKAe9ft1g?usp=sharing)


<div style="text-align: justify">Within months, COVID-19 went from an epidemic to a pandemic. From the first identified case in December 2019, how did the virus spread so fast and widely? The spread of disease is a real concern for a world in which global travel is commonplace.
Aware of the serious situation, with this quick project I will build a mini dashboard to quickly update the global situation across the globe provided open data and using open source libraries.
https://towardsdatascience.com/@nik.piepenbreier 
I’ll be using data from this wonderful Github repository that auto-updates the data daily. I’ll load our data into a Pandas’ dataframe based on the URL so that it’ll update automatically for us every day.</div>

<img src="images/covid19_visual.png" align="center"/>

---
## Data Science

### Bayesian Data Analysis


### DR. SEMMELWEIS AND THE DISCOVERY OF HANDWASHING
[![Run in Google Colab](https://img.shields.io/badge/Colab-Run_in_Google_Colab-blue?logo=Google&logoColor=FDBA18)](https://colab.research.google.com/drive/1zfnFEcGlq7zeNKT76TwMDrDIcwNQ69S_#scrollTo=wvnK9JanM5tE)


<div style="text-align: justify">In this notebook, we're going to reanalyze the data that made Semmelweis discover the importance of handwashing. Let's start by looking at the data that made Semmelweis realize that something was wrong with the procedures at Vienna General Hospital.</div>

<img src="images/Semmelweis.png" align="center"/><img src="images/handwashing.png" align="center"/>
---
<center>© 2020 Duy Nguyen. Powered by Jekyll and the Minimal Theme.</center>
