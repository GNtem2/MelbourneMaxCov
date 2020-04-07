# MelbourneMaxCov
Recent advances in acute stroke therapy has placed focus on transportation of patients to the appropriate hospital for acute stroke therapy. Some hospitals are capable of providing clot busting drug TPA only and selected hospitals are capable of providing clot busting drug TPA as well as clot extraction (ECR).Development of an equitable stroke service needs to optimize for hospital catchments and population at risk. The aim of this project is to perform a redundancy analysis by searching locations in Melbourne in which there are oversupply of stroke services. 

Travel time from the centroids of each suburbs to the (2 ECR designated hubs (ECR-Hub), 3 ECR capable (ECR-Capable) and 5 thrombolysis) hospitals is estimated using ggmap package in R to interface with Google Maps application program interface (API). Suburbs were assigned membership of a hospital if it is within 30 minutes. Next, we sequentially remove thrombolysis capable hospitals and examine the effect on service catchment. The population serviceable by each hospital was estimated using stroke incidence studies in Melbourne. 

The majority of suburbs (141 of 174 or 81.0%) are within 30 minutes catchment of at two or more ECR hubs and 96.6% (168/174) are within 30 minutes of all ECR hubs or thrombolysis capable hospitals. The median coverage by ECR hub is 3 (IQR 2, 4) [click here](./ECR.png) and ECR or thrombolysis is 4 (IQR 3 , 6) [click here](./TPAanECR.png). These suburbs are located within inner east Melbourne and are displayed below [![here](./MelbourneECR.png)](./MelbourneECR.html).

The picture is the same when both TPA and ECR hospitals are considered together [![here](./MelbourneTPA.png)](./MelbourneTPA.html)

Removing the thrombolysis capable hospitals in Melbourne only reduced the number of suburbs with redundant (≥2 hospital) coverage by 15.6%.

```github
git push -u origin master
```