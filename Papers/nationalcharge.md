---
title: "National Charge: Canadian Federal EV Standards Regulation"
draft: false
tags:
  - Paper📃
aliases:
  - Alexandre DesAulniers
---
#### Canadian Future Installation of Battery Electric Vehicle (BEV) and Plug-In Hybrid Vehicle (PHEV) Charging Infrastructure

Alexandre DesAulniers | March 2024 | [PDF](https://drive.google.com/file/d/1bH2xpy_td0OzaSvsQl2PB49UblCwcb_n/view?usp=sharing)

>[!abstract] 
>The following recommendation report delivers a recommendation on national ZEV charging standards based on evidence provided by Canadian consumers, national regulatory bodies, vehicle charging providers, automotive manufacturers, and patterns of international success. This assessment will build off the work of other national findings and global growing pains. Particularly, this report will be influenced by assessments submitted to National Resources Canada by Dunsky Energy and Climate Advisors on March 1st 2022 (Dunsky, 2022). Previous reporting has primarily focused on the national rollout of DCFC infrastructure, and national regulation on vehicle charging voltage regulation. While being a very positive and necessary recommendation, previous reportings are missing the primary scope to which this report of recommendation will address, that being electric vehicle connector charging standards. 
>
>The following charging standards will be assessed on a series of appropriate, and relevant criteria, based on data found from select sources that have been properly vetted for bias, and provide purely technical and nonpartisan data. Preference will be given to data collected by Canadian national bodies such as National Resources Canada, Transport Canada, and Statistics Canada. After careful consideration and comparison, SAE J3400 NACS has been chosen as this report's recommendation due to findings and comparisons of reliability, flexibility, and ease of use. 

^0450a1

  ---
  


## Table of Contents 

- [[nationalcharge#^0450a1|Abstract]]
- [[nationalcharge#Lists Of Figures and Tables|Lists of Figures and Tables]]
	- [[nationalcharge#​​List of Figures|Lists of Figures]]
	- [[nationalcharge#Lists of Tables|Lists of Tables]]
1. [[nationalcharge#1. Introduction|Introduction]] 
2. [[nationalcharge#2. Problem Background|Problem Background]] 
	2.2. [[nationalcharge#2.2 Evaluative Criteria|Evaluative Criteria]]
	  2.2.1 [[nationalcharge#2.2.1 Criteria Assessment Details Reliability and Cost|Criteria Assessment Details: Reliability and Cost ]]
	  2.2.2 [[nationalcharge#2.2.2 Criteria Assessment Details User Experience|Criteria Assessment Details: User Experience ]]
	  2.2.3 [[nationalcharge#2.2.3 Criteria Assessment Details Charger Installation Flexibility|Criteria Assessment Details: Charger Installation Flexibility ]]
3. [[nationalcharge#3. Evaluation of the SAE J1772/CCS Charging Standard|Evaluation of the SAE J1772/CCS Charging Standard]] 
	3.1 [[nationalcharge#3.1 SAE J1772/CCS Charging Standard Reliability and Cost Assessment|SAE J1772/CCS Charging Standard Reliability and Cost Assessment]]
	3.2 [[nationalcharge#3.2 SAE J1772/CCS Charging Standard User Experience|SAE J1772/CCS Charging Standard User Experience]]
	3.3 [[nationalcharge#3.3|SAE J1772/CCS Charging Standard Charger Installation Flexibility]] 
4. [[nationalcharge#4. Evaluation of the SAE J3400 NACS Charging Standard|Evaluation of the SAE J3400 NACS Charging Standard]]
	4.1 [[nationalcharge#4.1 SAE J3400 NACS Charging Standard Reliability and Cost Assessment|SAE J3400 NACS Charging Standard Reliability and Cost Assessment]]
	4.2 [[nationalcharge#4.2 SAE J3400 NACS Charging Standard User Experience|SAE J3400 NACS Charging Standard User Experience]]
	4.3 [[nationalcharge#4.3 SAE J3400 NACS Charging Standard Charger Installation Flexibility|SAE J3400 NACS Charging Standard Charger Installation Flexibility]]
5. [[nationalcharge#5. Evaluation of the TEPCO CHAdeMO Charging Standard|Evaluation of the TEPCO CHAdeMO Charging Standard]]
	5.1 [[nationalcharge#5.1 TEPCO CHAdeMO Charging Standard Reliability and Cost Assessment|TEPCO CHAdeMO Charging Standard Reliability and Cost Assessment]]
	5.2 [[nationalcharge#5.2 TEPCO CHAdeMO Charging Standard User Experience|TEPCO CHAdeMO Charging Standard User Experience]]
	5.3 [[nationalcharge#5.3 TEPCO CHAdeMO Charging Standard Charger Installation Flexibility|TEPCO CHAdeMO Charging Standard Charger Installation Flexibility]]
6. [[nationalcharge#6. Comparison of Results|Comparison of Results]]
7. [[nationalcharge#7. Conclusion/Recommendation|Conclusion/Recommendation]]

- [[nationalcharge#Glossary of Terms|Glossary of Terms]]
- [[nationalcharge#References|References]]




# Lists Of Figures and Tables

  


## ​​List of Figures 



- Figures 1-4:  [[nationalcharge#^f9640d|Commonly found Canadian electric vehicle charging standards, adapted from (N.R Canada, 2023) ]]

- Figure 5: [[nationalcharge#^a1a7a2|Makeup of Canadian electric charging network (adapted from Transport Canada, 2024)]]

- Figure 6: [[nationalcharge#^9c60d3|North American ZEV charging infrastructure failure rate by operator (adapted from J.D. Power, 2023)]]

- Figure 7: [[nationalcharge#^7278b7|New ZEV vehicle registrations, by charging standard, Q4 2022 — Q2 2023 (adapted from Statistics Canada, 2024)]]

- Figure 8: [[nationalcharge#^f8f82a|SAE J3400 NACS connector pinout interface (Tesla, Inc, 2022)]]

- Figure 9: [[nationalcharge#^2e6929|TEPCO CHAdeMO connector pinout interface (adapted from Mliu92 & Wikimedia Commons, 2021)]]



## Lists of Tables 



- Table 1: [[nationalcharge#^ebce1a|Example Decision Matrix and Assessment Scheme based on Assessed Criteria]]

- Table 2: [[nationalcharge#^507fba|Results from the University of California, Berkeley, Bay Area CCS functionality survey.]]

- Table 3: [[nationalcharge#^950791|Level 2 J1772 Charging Time versus a comparable Level 3 CCS DCFC charging station on a reference Hyundai Ioniq 5 (Hyundai Motor America, 2021)]]

- Table 4: [[nationalcharge#^c711f1|Key Points of each Assessment Criteria Overlaid on Decision Matrix]]

- Table 5: [[nationalcharge#^2cd7c4|Completed Decision Matrix and Assessment Scheme based on Assessed Criteria ]]

  ---
  


# 1. Introduction 


  

As millions of Canadians have moved towards, or are planning to purchase fully electric (BEV), plug-in hybrid vehicles (PHEV), or other ZEV vehicles, major growing pains are being identified nationwide. Canada’s infrastructure is not currently prepared to handle the influx of electric vehicles (N.R Canada, 2023). As public interest grows, and investment in the sector continues to expand, it will become increasingly important that strong foundations are set now to accommodate future developments on Canada’s roadways. The fragmentation of national and commercial resources on the front of sustainable transportation is a colossal inefficiency on the right path of national sustainability efforts. Electric vehicle charging standards have been a considerable sore spot when it comes to fragmentation of federal and commercial resources, with the high costs of deployment and maintenance being spread across standards. This has left hundreds of thousands of North Americans out when public and private spending is spent on a certain standard versus another (National Renewable Energy Laboratory, 2023).

With the current 2050 national net-zero mandate of greenhouse gas emissions set by the Government of Canada, and the recently amended national target of 100% ZEV sales of consumer passenger vehicles, it is peril that we make decisions on ZEV standards now, as setting forward precedent is now a must. 

This report aims to promote the standardization of a single national charging standard, and provide a basis for a potential future federally mandated charging standard. Any information sourced from a party potentially influenced by a particular agenda, or which has something to gain from a certain result, will be properly communicated as such to the reader. 



# 2. Problem Background



  

Across Canada, millions of Canadians are now entering the maturing, yet not settled, ZEV market. With huge automotive players such as Tesla, Ford, Hyundai, Toyota, and Chevrolet betting heavily on ZEV vehicles, and billions of dollars of national investment entering the electric vehicle market over the past decade, the success of electric vehicles is all but guaranteed (KPMG International LLP et al., 2021). However, Canadian regulatory bodies, and automotive manufacturers have yet to decide on a standardized charging format for the Canadian market.  The Canadian market presents interesting challenges for the deployment of ZEV‘s and their respective charging requirements. The Canadian winter climate challenges conventional global charging practices, and Canadian consumers require flexibility in where they charge their electric vehicles.

Whether that be on the side of a Trans-Canada highway, or in Canadian homes, if a unified charging standard is to be decided on, it must fulfill the requirements needed by Canadian drivers and the Canadian climate. 



## 2.1 Potential Solutions




Currently, there are three major competing standards in the Canadian electrical vehicle market. Those being the SAE J1772/CCS Connector, the SAE J3400 NACS North American Charging Standard, commonly known as “supercharger” and the TEPCO CHAdeMo connector. It should be noted that the SAE J1772/CCS Connector can be found in two forms, standalone J1772, and combined CCS meant for high power delivery deployments. Diagrams of each connector standard can be found below:

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcoh8a94NOkriZtLZNq-GYfwN8JewytIYP5j7cKe1lMl9IZStbW2h4VHk8D8livt3Uw0yiQD9mwPzJES4RM4U-QdwTVmVNq5jpG-hMTCBoSP4litTEglb92lz5rsjhy1pf-j6CYdiULc_HhvxMs70tk-XSB?key=qAJ-MzjNJ9DUxc6fdkXQ9g)

##### Figures 1-4:  Commonly found Canadian electric vehicle charging standards, adapted from (N.R Canada, 2023)



## 2.2 Evaluative Criteria



The following charging standards will be assessed on the following criteria:  

- Reliability/Cost
    
- User Experience 
    
- Charger Installation Flexibility


The following table describes the weight of each assessment criteria for the following report’s assessment:

#### Table 1: Example Decision Matrix and Assessment Scheme based on Assessed Criteria

|                        |                  |                 |                                  |       |
| ---------------------- | ---------------- | --------------- | -------------------------------- | ----- |
|                        | Reliability/Cost | User Experience | Charger Installation Flexibility | Total |
| SAE J1772/<br><br>CCS  | 5                | 5               | 5                                | 15    |
| SAE J3400 <br><br>NACS | 5                | 5               | 5                                | 15    |
| TEPCO CHAdeMo          | 5                | 5               | 5                                | 15    |


Each evaluation criteria will be assessed out of five points, for a total possible fifteen points.  Additional notes will be made throughout the recommendation report in each criteria’s respective subsection, including that of potential manufacturer bias, and data sourcing concerns. Certain data points will be sourced from vehicle manufacturer datasets, and in turn, will be valued less in the event of conflicting information. Data reported from national federal bodies such as Transport Canada, Statistics Canada, and Natural Resources Canada will be taken into primary consideration, followed by international standards groups such as SAE International and the CSA Group. No dataset will be taken into consideration prior to 2022, as rapid development in the ZEV market quickly creates dated information. Miles, D. (2010) is an exception, as the data provided is still relevant. Constant development and standard revision in the past ten years have vastly changed the capabilities of ZEV charging standards. 



### 2.2.1 Criteria Assessment Details: Reliability and Cost


  

Reliability will be primarily assessed on connector design, repairability complexity and historical reliability data. Cost will be primarily assessed on total residential installation cost and total commercial DCFC installation cost, but will also be assessed on upfront and continuing licensing costs, repair costs, and other associated lifetime upkeep costs. Data to evaluate reliability has been primarily sourced from SAE International (2021), CSA Group (2022), Rempel et al (2022), Evie Networks (2022) and Tesla, Inc (2022), with prudence to insure fair comparison. Data collected from Tesla’s technical specification report regarding the SAE J3400 NACS standard will be evaluated purely from a perspective of reported technical information, and not opinion. 



### 2.2.2 Criteria Assessment Details: User Experience


  

The user experience assessment will be primarily assessed on the ease of use of the charging standard, current reported vehicle port usage, new vehicle sales by port, and charge times. Data will be primarily sourced from current Transport Canada (2024) public national infrastructure figures, Statistics Canada, (2024) market share reports and Canadian Automobile Association & Plugshare Research (2023) customer satisfaction surveys. Primary charge time data will be sourced from Hyundai Motor America, (2021), CHAdeMO Association, (2020), and Tesla, Inc (2022). 



### 2.2.3 Criteria Assessment Details: Charger Installation Flexibility




The charger installation flexibility criteria will primarily be assessed on the versatility of use case ranges, and possible deployment limitations. This section will include extra information on residential deployments, commercial DCFC installations, and portable charging standards and solutions. Data will be primarily collected from SAE International (2021), Hyundai Motor America (2021) and Tesla, Inc (2022). 



# 3. Evaluation of the SAE J1772/CCS Charging Standard



The SAE J1772 connector standard was drafted and detailed in the initial J1772 standard, SAE J1772-2001. The SAE J1772 connector was created in response to the California Air Resources Board’s (CARB) request for a standardized electric vehicle connector. The SAE J1772 connector project was then given to the electric vehicle research board, AVCON, and was published in June 2001. Since the J1772-2009 revision in June 2009  SAE International has been the main regulatory body tasked with the future development of the connector. (California Air Resource Board | CARB, 2001). 

Developed as part of the J1772-2009 revision, SAE International introduced the J1772/CCS Combo coupler, which added CCS high voltage direct current expansion to the J1772 standard. The CCS standard is in wide use today, by automotive manufacturers such as Hyundai Automotive, The Volkswagen Group, Mercedes-Benz Group and Nissan Motor (Coordination Office Charging Interface c/o Carmeq GmbH, 2011). CCS has been the backbone of Canadian high speed direct current charging, and has been the driving force behind the open standard high voltage direct current effort throughout the past decade (Statistics Canada, 2024). There are two variants of the CCS standard, however, this report will solely focus on the “Type 1” variant, developed for the North American domestic market.  



## 3.1 SAE J1772/CCS Charging Standard Reliability and Cost Assessment




The SAE J1772/CCS Combo charging standard has been in full effect since November 2011, and since then, has proven itself as a connector since its inception in the J1772-2009 standard revision. It can deliver stable power up to 350 kW, with complete safety (SAE International, 2021). A study done by the Department of Bioengineering, University of California, Berkeley in 2022 determined that J1772/CCS Connector equipped charging stations in the Greater Bay Area were fully functional 72.5% of the time over the course of the year of study. However, of those failures, it was reported that connector faults occurred only 0.9% percent of the time. This study was conducted using random charging intervals and 657 recorded charging stations. The study also included  public survey data, which reported that the Greater Bay Area population reported a charger connector related failure rate of 9%. The overwhelming majority of cases of non-functioning chargers (98.2%) of failures were related to payment terminals, non responding touch screens or charging terminals, and not the charging connector itself (Rempel et al., 2022). 

Below, are the complete findings of the University of California, Berkeley study:


#### Table 2: Results from the University of California, Berkeley, Bay Area CCS functionality survey.

#### ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeoAzt2REA52ZBnuJRC5js7ToWw_uCNRedszVnZJMqZ5qPb3NvcGc_D4efgKoqM7UM1HWs-BP8J5zLqZ247r4J6iRjGDcs_TLVuWIrZH3hS71w7St6Lz4kaWxXXNO6JjX4Zmg9TCcBK-phRzlJ2?key=qAJ-MzjNJ9DUxc6fdkXQ9g)

The University of California, Berkeley report is considered to be one of the most credible sources of J1772/CCS reliability, and aligns with other consumer reports. The J1772/CCS connector proves robust, but is known to have issues regarding the connector clip cracking, and is frequently accompanied by underfunded public infrastructure. This has unfortunately cast a negative image on the J1772/CCS connector, and is an ongoing national issue which will continually improve (Rempel et al., 2022). The J1772/CCS connector is designed to be robust, and operate seamlessly in both direct current, and alternating current modes for residential use. It has seen many revisions over the past decade, and has a very large adoption rate. Average commercial DCFC installation rates approximate $10,000 —  $40,000, while level 2 residential connections average cost $1000 — $2000, and level 2 commercial installations average $2,000 — $10,000. (CSA Group, 2022)



## 3.2 SAE J1772/CCS Charging Standard User Experience




The SAE J1772/CCS Charging Standard is by far the most popular charging standard in Canada, accounting for 83.1% of all available charging ports nationwide. 

Shown below is the makeup of the currently functional Canadian electric charging network:

  
  
  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfno-Myy_3o427J-C8Ha9E9GmlftZMU4uGlSb2BXDMENJ9-k2CEBJNUHLyT7zHqDOS90DNETm993-nQHcLL2TPHAHEP-2F_SVYlS4fFb8wULKdu3ajOpbaQVXZacT3XgefBmw7QOKP2uuQDZrXY-WOEi_Vt?key=qAJ-MzjNJ9DUxc6fdkXQ9g "Canadian Electric Vehicle Charging Port Adoption")

  
  
  

##### Figure 5: Makeup of Canadian electric charging network (adapted from Transport Canada, 2024)


With over 24,627 public J1772/CCS charging connectors across Canada, J1772/CCS is by far the most widely adopted connector nationwide. An owner of a vehicle with a J1772/CCS connector would have a huge amount of public charging infrastructure to use, while also being able to charge their vehicle at home. According to Transport Canada (2024), 74.6% of new ZEV vehicles sold utilized a J1772/CCS charger. Being the market leader gives J1772/CCS a huge advantage in early adoption, and existing infrastructure. 

However, the full speed J1772/CCS combo charger is a large connector, comprising two separate connectors. During level 1 and level 2 charging, which are the only options for residential charging, solely the J1772 connector is used (Miles, 2010). This is a smaller connector, however, J1772 is limited to 19.2 kW instead of the full 350KW capable by the CCS combo connector (SAE International, 2021). 

For a reference Hyundai Ioniq 5, which, as per Transport Canada (2024), is Canada's most popular J1772/CCS equipped BEV, the difference in charging time is significant. 

Below is a charging comparison table comparing level two J1772, and level three CCS DCFC on the 2022 Hyundai Ioniq 5: 


#### Table 3: Level 2 J1772 charging time versus a comparable level 3 CCS DCFC charging station on a reference Hyundai Ioniq 5 (Hyundai Motor America, 2021)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeps9UrGBYF4g5QIDROGuoz6qaCnTnaTAlTmGLfAuYg69oMTiRXYhT7oFe0zHoiSkX_1OfgM79uwfsSxpQCeR3moT9Uu3I0PTIkJnkOz9L35YJtwMURVb-94EGqSQcPUMXF9NgTRmw0OyrZiMmy8smWfKQ6?key=qAJ-MzjNJ9DUxc6fdkXQ9g)

  
To achieve the full charging speed of the reference Hyundai Ioniq 5, a full CCS DCFC  connector is needed, meaning that the driver must use the large connector combo. This may cause confusion among unfamiliar users who expect rapid charging at public Canadian charging stations.


  
## 3.3 SAE J1772/CCS Charging Standard Charger Installation Flexibility




SAE J1772/CCS has proven to be a very diverse standard, and can be deployed across many differing climates and installations. However, it is important to note that the additional CCS combo plug is used solely at DCFC stations, and not in residential installations. Residential J1772 is limited to 240V, 48A which is the limit of the vast majority of Canadian households. Level two charging usually requires additional electrical work to an average Canadian household as well, and will add additional cost. A level one 120V, 16A, which can be plugged into a standard Canadian AC outlet typically comes with the purchase of a ZEV vehicle, and can be used without additional cost. (CSA Group, 2022) The J1772/CCS standard will always negotiate the highest pre-determined safe charging speed capable by both the power source, and the receiving vehicle. While the three different tiers of charging of the SAE J1772/CCS may prove confusing to an unaware consumer, it has proven to be a very versatile and capable standard. (Canadian Automobile Association & Plugshare Research, 2023)



# 4. Evaluation of the SAE J3400 NACS Charging Standard


  

Being the newest standard compared, the NACS North American Charging Standard is currently in the process of being standardized by SAE International as SAE J3400. NACS was created in 2012 by Tesla, Inc as the primary, and later only method of charging Tesla branded vehicles. NACS began the standardization process in 2022, with SAE International announcing adopting in June 2023, partnering with Volex Manufacturing as the primary manufacturing partner. The SAE J3400 NACS standard is planned to be finalized in the fall of 2024 (SAE International, 2023).

SAE J3400 NACS is currently in an unfinalized state, which proves it difficult to fully evaluate. While in its current state, it can be evaluated with Tesla and Ford vehicles, the standard hasn’t been fully implemented widely. In the present day, NACS is fully managed by Tesla, Inc. However, once finalization of the SAE J3400 standard is completed, SAE International will assume full responsibility for future development and revisions of the standard. (SAE International, 2023)



## 4.1 SAE J3400 NACS Charging Standard Reliability and Cost Assessment




Like the SAE J1772/CCS Combo standard, prior to the SAE J3400 standardization, the NACS standard has proven itself to be very reliable and capable for Canadian consumers since its initial deployment in 2012 (Canadian Automobile Association & Plugshare Research, 2023). Prior to the beginning of the SAE J3400 NACS standardization process, NACS had always enjoyed a very positive image in the light of reliability. 

According to J.D. Power (2023), Tesla-branded NACS stations experienced a North-American-wide station failure rate of 3.9% 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe6WfelIOVRRzouJs5jRxXtcAdNGDF3J9JzOrtWQN1UEtagLdZQMk5yDQ5iWzT4LSwSRKKPXyrvHTjqVJiULHKX6cvVzChF89X-dHc5QBJRyBW22TNwIAhQshgGZin9SUdXM2zZKbSDPRLFHCLgDGdk8Maw?key=qAJ-MzjNJ9DUxc6fdkXQ9g "% Respondents Unable to Charge by Charge Point Operator — 2023 Q1")

##### Figure 6: North American ZEV charging infrastructure failure rate by operator (adapted from J.D. Power, 2023)

At the time of data collection, Tesla branded NACS stations represented the vast majority of NACS public infrastructure. However, while this paints a broad picture of reliability, this data is not indicative of the problem at hand. Many have looked at these initial findings with the conclusion that the NACS protocol is the more reliable standard. However, it must be recalled that the results from the University of California, Berkeley charging reliability survey concluded that J1772/CCS connector failures represented 0.9% of total failures. 

The current situation is that charging terminals owned and operated by Tesla, Inc, which constitute the majority of national NACS terminals, are subject to a significant incentive to remain operational for Tesla's customer base. Tesla ensures that Tesla branded charging infrastructure is functional, and such reflects in national failure rates. This will be subject to change as NACS becomes standardized, and becomes available to all charging network operators. 

Level two residential NACS charging solutions will cost $1000 — $2000, while level two commercial installations average $2,000 — $10,000 (CSA Group, 2022). There is currently no public information about total commercial DCFC installation cost, and no current public information about future licensing costs. 


  
## 4.2 SAE J3400 NACS Charging Standard User Experience


  

While having a much lower market share compared to the general J1772 standard, NACS is competitive with CCS in terms of high speed DCFC charging market share, as shown below:

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfno-Myy_3o427J-C8Ha9E9GmlftZMU4uGlSb2BXDMENJ9-k2CEBJNUHLyT7zHqDOS90DNETm993-nQHcLL2TPHAHEP-2F_SVYlS4fFb8wULKdu3ajOpbaQVXZacT3XgefBmw7QOKP2uuQDZrXY-WOEi_Vt?key=qAJ-MzjNJ9DUxc6fdkXQ9g "Canadian Electric Vehicle Charging Port Adoption")


##### Figure 5: Makeup of Canadian Electric charging network (adapted from Transport Canada, 2024)

This fact is also reflected in new ZEV market share statistics, as provided by Statistics Canada new national vehicle registrations: 

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcx5L9lk83eEKDMjRooSRBwB4huur4hzLjZ5_-LRHFo8fZifqQ1vKCIRhk1dzKDjXC0ywXQdfaCPuBb-Np_dNpO27bhuAg5qEf_X-VUv1GzogdbyNSCotFRjf43UF1tb97XqQQg3mlR3fKZelKWEzZ0Cl1T?key=qAJ-MzjNJ9DUxc6fdkXQ9g)

  

##### Figure 7: New ZEV vehicle registrations, by charging standard, Q4 2022 — Q2 2023 (adapted from Statistics Canada, 2024)

While national NACS charging infrastructure is comparatively small in terms of total national installation rates, DCFC  installations remain high. These rapid charging DCFC installations are what Canadian consumers benefit from the most, as they are mostly the only viable option while travelling long distances in Canada without charging overnight. Rivalling CCS in terms of DCFC market share allows NACS to be a very appealing option to Canadian consumers, even prior to SAE J3400 standardization. With high DCFC adoption rates, and NACS occupying over 25% of new ZEV market share, Canadian customers will continue to have many options for vehicle charging. NACS can provide up to 1,000V, 350KW, making it comparable in charging time to a comparable CCS system (1000V) (Tesla, Inc, 2022). 



## 4.3 SAE J3400 NACS Charging Standard Charger Installation Flexibility




Similarly to the SAE J1772/CCS standard, SAE J3400 NACS can be deployed in both high voltage DC, and 240v/120v residential AC environments. However, the SAE J3400 NACS has the massive advantage of being completely functional in DCFC deployments as one connector. This is in contrast to SAE J1772/CCS, which requires both J1772, and CCS connectors to achieve the maximum of 350KW (Miles, 2010).  This gives SAE J3400 NACS an advantage in size over SAE J1772/CCS, resulting in a connector that is mechanically simpler. The above factors result in SAE J3400 NACS being a less intimidating, and less complicated connector to use for the consumer. As long as the consumers' vehicle has the accompanying port, SAE J3400 NACS will automatically negotiate charging speed. (Tesla, Inc, 2022)

Shown below are side by side figures comparing the size of both SAE J1772/CCS and SAE J3400 NACS: 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcoh8a94NOkriZtLZNq-GYfwN8JewytIYP5j7cKe1lMl9IZStbW2h4VHk8D8livt3Uw0yiQD9mwPzJES4RM4U-QdwTVmVNq5jpG-hMTCBoSP4litTEglb92lz5rsjhy1pf-j6CYdiULc_HhvxMs70tk-XSB?key=qAJ-MzjNJ9DUxc6fdkXQ9g)

##### Figures 2 & 3: SAE J1772/CCS Combo (Labelled “CCS1”) in comparison to the SAE J3400 NACS (Labelled “Supercharger”) connector (adapted from N.R Canada, 2023)

SAE J3400 NACS is capable of being compact due to its ability to deliver both AC and DC power over the same pins of the connector. AC/DC power is delivered over the top two pins, while ground is configured to the middle lower pin. Communication from terminal to vehicle is handled via the two remaining lower pins (Tesla, Inc, 2022). 

An electrical diagram can be seen below of SAE J3400 NACS’s 5 pin configuration:

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXexw_cXCn7Mp7xTmU1UhRoBUwg1Yl8Mui5hrZ99mmu7fYhgGBs1lyvlbn3LcdhmMdUfroLScUbN3ba1mWw5uyoSk460FJlRzX4E4WHAs-zQno2-gqSTPH908UMhOxNQEk0aezbrg31qo6ygntiRX1ifueuY?key=qAJ-MzjNJ9DUxc6fdkXQ9g) 

##### Figure 8: SAE J3400 NACS Connector Pinout Interface (Tesla, Inc, 2022)
  
The SAE J1772/CCS standard delivers high voltage DC over the two lower large pins provided by the CCS extension, while charging communication and AC power delivery take place over the main J1772 portion of the connector. This is the reason for the large size of the combo J1772/CCS standard.



# 5. Evaluation of the TEPCO CHAdeMO Charging Standard


  

Established in 2010 by the Tokyo Electric Power Company (TEPCO), CHAdeMO was one of the earliest pioneers in the DCFC rapid charging market. CHAdeMO is a high voltage DC bidirectional charging standard backed by Japanese manufacturers Subaru, Mitsubishi Heavy Industries, and Panasonic, and is currently maintained by the CHAdeMO Association and TEPCO. (CHAdeMO Association, 2022). CHAdeMO has struggled with mass adoption in the North American market since its inception, however, enjoys large market share in eastern Asian regions such as Japan (96%) (Shimizu et al., 2023). The CHAdeMO standard is currently the only standard available globally with the ability to accommodate V<sub>2</sub>G grid buyback technologies, which Japan has proven itself very open to. (CHAdeMO Association, 2022)

Introduced in June 2018, CHAdeMO 2.0 was a revision aimed at raising charging speeds to match competitors SAE J1772/CCS and SAE J3400 (400KW at 1000V). As of 2020, The CHAdeMO Association is partnering with the China Electric Council (CEC) to publish the CHAdeMO 3.0 specification, which will deliver up to 900KW of power at 1000V.  This standard has yet to be finalized. (CHAdeMO Association, 2022). 



## 5.1 TEPCO CHAdeMO Charging Standard Reliability and Cost Assessment


  

CHAdeMO, like SAE J1772 and NACS , has proven itself as a long time market player, with a large global presence. CHAdeMO has made huge commitments to user safety, with it being an integral design to the connector. Along with common circuit interruptions used by other global standards, it is one of the few to include a locking connection to the vehicle while charging. The receiving vehicle receptacle will lock itself to the CHAdeMO connector while charging, ensuring that it doesn’t come undone accidentally (CHAdeMO Association, 2020). Many have welcomed CHAdeMO’s innovative locking charging system, heralding it for the safety benefits it provides, however,  many users have been vocal about reported issues regarding the locking connector system and vehicles getting stuck while charging at public charging infrastructure (Tommy84 et al., 2021). CHAdeMO relies on the charging station to let it know when it finishes charging, and then releases itself from the vehicles. What can occur, is that when public charging infrastructure malfunctions or is broken, it will not let the connector know when it is done, therefore, not releasing the connector from the vehicle. Users may then have to wait for a charging network operator to then manually release the connector from the vehicle receptacle (Evie Networks, 2022). 

As well as the locking connector, CHAdeMO is also one of the most complex charging standards connection wise, having two power pins, and seven communication pins. CHAdeMO communicates over the same data protocol used by SAE J1772/CCS and SAE J3400 NACS. (CHAdeMO Association, 2020).

An electrical diagram can be seen below of the TEPCO CHAdeMO pin configuration:



![|500](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcjcKjmwBf60CxOwgvgAkKwkU_o5BH1MvGxmqjrryhl1geC2gR3_PGtdU-im4rqacC54VLeHiUs2mMWqZDHD14Atu2c4IJxIgl9e51TZBUg0d3BdL_lKCOeDHclu1lTucJOTDFwtrsteCkQXwBYM7TjNt0u?key=qAJ-MzjNJ9DUxc6fdkXQ9g)


##### Figure 9: TEPCO CHAdeMO Connector Pinout Interface (adapted from Mliu92 & Wikimedia Commons, 2021)

Average commercial DCFC 2 installation rates approximate $10,000 —  $40,000, which is a similar  cost to comparable SAE J1772/CCS installations (CSA Group, 2022). There are no residential A/C connections for CHAdeMO, as it is purely a DC standard.



## 5.2 TEPCO CHAdeMO Charging Standard User Experience




CHAdeMO offers a single cable solution for all voltages, similar to NACS. It is of similar profile to the NACS connector, and is remarkably easy to use. CHAdeMO is a remarkably safe and feature filled connector, with thoughts such as the locking charge receptacle, and V<sub>2</sub>G setting it apart from the competition (CHAdeMO Association, 2020). 

The primary obstacles faced by CHAdeMO in North America revolve around market share, plug availability, and the exclusive DC-only architecture of the standard. This eliminates CHAdeMO from the home market entirely, as the vast majority of North American homes can only provide 120/240V AC connections (Quick 220 Electrical Systems, n.d.). Reported public CHAdeMO infrastructure data made available by Transport Canada (2024), states that CHAdeMO connections only makes up 8.1% of Canada’s current charging ZEV infrastructure, and this number is declining each year. There have been no new market vehicle registrations for CHAdeMO-equipped vehicles in Canada as of the second quarter of 2023 (Statistics Canada, 2024). Without the use of charging adapters, this would make the use of a CHAdeMO equipped vehicle in Canada very difficult, with very limited charging options. 

Using a CHAdeMO 2.0 400KW connection, the CHAdeMO Association, (2022) claims that “it can feed the electricity necessary for 40 km drive within 5 minutes, and 60 km within 10 minutes. With 30 minutes, you can almost fully charge your EV”. No reference vehicle model was given. However, this figure would align with other known 400KW connections. 



## 5.3 TEPCO CHAdeMO Charging Standard Charger Installation Flexibility




CHAdeMO’s flexibility of installation is severely compromised by the connector's solely DC architecture. CHAdeMO cannot be used in Canadian residential installations due to the requirement of a high voltage DC input. The requirement of a high voltage DC input is a large barrier to national CHAdeMO adoption, as CHAdeMO would require significant investment into DCFC infrastructure to provide few public facing charging interfaces. CHAdeMO’s V<sub>2</sub>G capabilities, however, are very interesting. If proper infrastructure were to exist, CHAdeMO’s V<sub>2</sub>G would allow for massive gains to national grid stability, and would allow users to leverage the technology to power homes during periods of distress and grid instability. 



# 6. Comparison of Results




After careful review of each charging standard under a set of strictly reviewed criteria, the weights of each standard can now be reviewed and compared. 

A comparison chart of each standard can be seen below, filtered by criteria and flagged by items of note, drawbacks, and benefits. Items of note are noted in yellow, drawbacks are noted in red, and benefits are noted in green.

#### Table 4: Key Points of each Assessment Criteria Overlaid on Decision Matrix


<span style="background:#fff2cc">Items of Note</span> | <span style="background:#e6b8af">Drawbacks</span> | <span style="background:#d9ead3">Benefits</span>

|                |                                                                                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                                                               |                                                                                                                                                                                                                                                                            |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                | Reliability/Cost                                                                                                                                                                                                                                                                                                                                                                                                         | User Experience                                                                                                                                                                                                                                                                                                                                                                               | Charger Installation Flexibility                                                                                                                                                                                                                                           |
| SAE J1772/CCS  | <font color="#fff2cc">Reliable, however, associated with poor charging infrastructure</font><br>    <br><br><br><font color="#e6b8af">Clip Cracking issues</font><br>    <br><br>  <br><br><font color="#d9ead3">Various cost tiers, low to high</font>                                                                                                                                                                  | <font color="#fff2cc">Fast charging speed (350KW) </font><br>    <br><br>  <br><br><font color="#e6b8af">Multiple connectors needed for DCFC </font><br>    <br><br>  <br><font color="#d9ead3">Huge pre-existing infrastructure</font>                                                                                                                                                       | <font color="#fff2cc">Many options for diverse AC/DC installations</font><br>    <br><br><font color="#e6b8af">Current difficulty to determine fast charging infrastructure. </font><br>    <br><br><font color="#d9ead3">Scalable architecture</font>                     |
| SAE J3400 NACS | <font color="#fff2cc">Reliable, however, not currently an open standard </font><br>    <br><br>  <br><font color="#e6b8af">Reliability data skewed, and the majority of charging infrastructure corporately owned by Tesla.</font> <br>    <br><br>  <br><br><font color="#e6b8af">DCFC and licensing costs, not yet clear.</font><br>    <br><br>  <br><br><font color="#d9ead3">Various cost tiers, low to high</font> | <font color="#fff2cc">Fast charging speed (350KW)</font><br>    <br><br>  <br><br><font color="#e6b8af">Overall lower current national adoption</font><br>    <br><br>  <br><br><font color="#d9ead3">High/Comparable DCFC adoption<br>    </font><br><br>  <br><br><font color="#d9ead3">Growing market share</font><br>    <br><br>  <br><br><font color="#d9ead3">Single Cable DCFC</font> | <font color="#fff2cc">Many options for diverse AC/DC installations</font><br>    <br><br>  <br><br><font color="#d9ead3">Mechanically simpler compared to competition</font><br>    <br><br>  <br><br><font color="#d9ead3">Small, sleek, easy-to-use charging port</font> |
| TEPCO CHAdeMo  | <font color="#fff2cc">Reliable, with an emphasis on user safety<br>    </font><br><br>  <br><br><font color="#e6b8af">Connector locking while using poorly maintained public infrastructure </font><br>    <br><br>  <br><br><font color="#e6b8af">Mechanically quite complicated</font><br>    <br><br>  <br><br><font color="#e6b8af">No cost tiers, with a high cost of entry</font>                                  | <font color="#fff2cc">Fastest Charging Speed (400KW)</font><br>    <br><br>  <br>  <br><br><font color="#e6b8af">Very low existing market share of vehicles and infrastructure</font> <br>    <br><br>  <br><br><font color="#d9ead3">Single Cable DCFC</font>                                                                                                                                | <font color="#e6b8af">Severely lacking options  for installation diversity</font><br>    <br><br>  <br><br><font color="#e6b8af">High voltage DC requirement</font><br>    <br><br>  <br><br><font color="#d9ead3">V<sub>2</sub>G Capabilities</font>                      |

  

Using these assessed noted points, with each criteria being weighted equally, point values can now be tallied up to provide an analytical conclusion for a strong forward recommendation for a potential future national charging standard.

An individual point breakdown of all evaluated criteria can be seen below:


#### Table 5: Completed Decision Matrix and Assessment Scheme based on Assessed Criteria


<font color="#d9ead3">Primary Recommendation</font> | <font color="#fff2cc">Secondary Recommendation</font> | <font color="#e6b8af">Not To Be Recommended</font>

|                        |                  |                 |                                  |                                    |
| ---------------------- | ---------------- | --------------- | -------------------------------- | ---------------------------------- |
|                        | Reliability/Cost | User Experience | Charger Installation Flexibility | Total                              |
| SAE J1772/<br><br>CCS  | 4/5              | 3/5             | 4/5                              | <font color="#c3d69b">11/15</font> |
| SAE J3400 <br><br>NACS | 3/5              | 4/5             | 5/5                              | <font color="#d9ead3">12/15</font> |
| TEPCO CHAdeMo          | 2/5              | 2/5             | 1/5                              | <font color="#e6b8af">6/15</font>                               |

SAE J3400 NACS initially raised concerns of competition faltering, due to Tesla, Inc’s market position, and monopoly on NACS national charging. However, as NACS transitions into SAE J3400, and Tesla, Inc forgoing complete control of the standard, many primary concerns dry up. The SAE Group has demonstrated to be a reliable and fair party, which prioritizes current and future standard concerns and development over immediate profit. SAE J3400 NACS  has proven to be a strong market contender, and will be the primary recommendation of this report. 

SAE J1772/CCS struggles with additional complexities regarding the J1772 and CCS connector separation, causing possible customer uncertainty and confusion about charging rates, increased size, and additional failure points. SAE J1772/CCS remains a very reliable standard and would be worthy of a secondary recommendation for many of the same reasons as SAE J3400 NACS. 

Those benefits being:

- High percentage of currently installed DCFC infrastructure 
    
- Current market share percentages 
    
- Existing infrastructure and installation rates
    
- Diversity of infrastructure deployment.
    

TEPCO CHAdeMO cannot be recommended for the Canadian market almost solely due to the connector’s uniquely DC only architecture, severely limiting national deployment options. This was compounded by:

- Low existing Canadian adoption rates 
    
- High voltage DC requirements increasing barriers to entry
    
- Connector Issues 
    
- Nonexistent in North American ZEV market share
    

While V<sub>2</sub>G is an interesting and potentially very useful future technology, the cost to Canadian consumers now would be unavoidable, and not completely necessary. CHAdeMO would demand much more change on Canadian grids than what can currently be done, and the benefits would not amount to the cost incurred. 


# 7. Conclusion/Recommendation

  

After careful consideration and comparison, SAE J3400 NACS has been chosen as the wholly recommended potential future national charging standard to begin Canada-wide standardization. 

The rationale behind this conclusion was based on:

- Superior connector design for simplicity, high voltage transfer and reliability 
    
- High percentage of currently installed DCFC infrastructure
    
- Q2 2023 Market share percentages, and increasing availability on ZEV‘s
    
- Diversity of AC/DC commercial and residential deployments
    
- Strong reliability track record 
    

Once fully standardized, SAE J3400 NACS will fully complete all criteria sought out by Canadian regulators and consumers. SAE J3400 NACS will prove to be a long-lasting, dependable standard for electric vehicles in Canada, with public and industry backing alike. 

---
# Glossary of Terms

3 — BEV

Battery Electric Vehicle, as labelled by Transport Canada. Fully electric central battery operated vehicle, with zero emission, or employment of any fossil fuels. 


2 — DCFC

Direct Current Fast Charging. High voltage direct current rapid charging stations, Typically publicly accessible, and meant to be generally used along roadway or highway infrastructure 

  
5 — NACS

North American Charging Standard, as labeled by Tesla, Inc. Also, commonly known as the “Tesla Supercharger”. NACS is a private standard, owned by Tesla, Inc which is currently in the process of transitioning into an open standard known as the SAE J3400 North American Charging Standard, which will be managed by international standards group SAE Group. 


4 — PHEV

Plug-In Hybrid Electric Vehicle, as labelled by Transport Canada. Typically, shorter range electric vehicles, which switch to a hybrid electric/fossil fuel drive model once the battery cells have been depleted. Must have a dedicated charging port to be considered a PHEV.

  
6
—  V<sub>2</sub>G

Vehicle To Grid is a technology which allows vehicles to contribute electricity back into a power grid to compensate for times of high grid demand, and to add general grid resiliency.   

  
1 —  ZEV

   Zero Emissions Vehicle, as labelled by Transport Canada. A vehicle which produces zero emissions while in operation. 

---
# References



California Air Resource Board {CARB}. (2001). Adoption of amendments to the California zero-emission vehicle regulations: treatment of majority owned small and intermediate volume manufacturers and standardization of charging systems for the zero emission vehicle program. In California Air Resource Board (CARB). [https://ww2.arb.ca.gov/sites/default/files/barcu/regact/charger/uid.pdf](https://ww2.arb.ca.gov/sites/default/files/barcu/regact/charger/uid.pdf)

Canadian Automobile Association & Plugshare Research. (2023). The voice of the Canadian electric vehicle driver. In www.caa.ca. [https://www.caa.ca/app/uploads/2023/06/CAA-Canadian-EV-Driver-Study_FINAL_EN.pdf](https://www.caa.ca/app/uploads/2023/06/CAA-Canadian-EV-Driver-Study_FINAL_EN.pdf)

CHAdeMO Association. (2020). CHADeMO Mission Statement. In CHAdeMO.com. [https://www.chademo.com/wp/pdf/3-1-Mission%20statement-long.pdf](https://www.chademo.com/wp/pdf/3-1-Mission%20statement-long.pdf)

CHAdeMO Association. (2022, June). History of the CHAdeMo Organization. CHAdeMo. [https://www.chademo.com/about-us/organisation](https://www.chademo.com/about-us/organisation)

Coordination Office Charging Interface c/o Carmeq GmbH. (2011, November 8). Combined Charging Current status of the combined charging system {Slide show; Web}. Daimler Automotive. [https://web.archive.org/web/20120426054301/http://www.ishavsveien.no/wp-content/uploads/2011/11/Current_status_of_the_Combined_Charging_System_v1.2.pdf](https://web.archive.org/web/20120426054301/http://www.ishavsveien.no/wp-content/uploads/2011/11/Current_status_of_the_Combined_Charging_System_v1.2.pdf)

CSA Group. (2022). Charging Ahead: Ensuring equity and reliability in Canada’s electric vehicle network. In CSA-Charging Infrastructure Public Policy Report. [https://www.csagroup.org/wp-content/uploads/CSA-ChargingInfrastructure-PublicPolicyReport-EN_Accessible.pdf](https://www.csagroup.org/wp-content/uploads/CSA-ChargingInfrastructure-PublicPolicyReport-EN_Accessible.pdf)

Dunsky. (2022). Canada’s public charging infrastructure needs. In National Resources (N.R) Canada. National Resources (N.R) Canada. [https://natural-resources.canada.ca/sites/nrcan/files/energy/cpcin/2022-ev-charging-assesment-report-eng.pdf](https://natural-resources.canada.ca/sites/nrcan/files/energy/cpcin/2022-ev-charging-assesment-report-eng.pdf)

Evie Networks. (2022, March 16). What to do if a CHAdeMO Connector Gets Jammed [Video]. YouTube. [https://www.youtube.com/watch?v=F8uv-ZA6A1U](https://www.youtube.com/watch?v=F8uv-ZA6A1U)

Hyundai Motor America. (2021). 2022 IONIQ 5 Specifications [Dataset; Web]. In Battery (Version V3). Hyundai Newsroom. [https://www.hyundainews.com/assets/documents/original/48175-2022Ioniq5ProductGuidespecs090821.pdf](https://www.hyundainews.com/assets/documents/original/48175-2022Ioniq5ProductGuidespecs090821.pdf)

J.D. Power. (2023). Ford and GM adoption of Tesla charging network addresses major consumer pain point, sets stage for battle about Fast-Charging standard. In J.D. Power. [https://www.jdpower.com/business/resources/ford-and-gm-adoption-tesla-charging-network-addresses-major-consumer-pain-point](https://www.jdpower.com/business/resources/ford-and-gm-adoption-tesla-charging-network-addresses-major-consumer-pain-point)

KPMG International LLP, Silberg, G., Suganuma, Y., Jullens, J., Dubner, T., & Shapiro, E. (2021). Place your billion-dollar bets wisely. In KPMG. KPMG International. [https://kpmg.com/kpmg-us/content/dam/kpmg/pdf/2023/place-your-billion-dollar-bets-wisely.pdf](https://kpmg.com/kpmg-us/content/dam/kpmg/pdf/2023/place-your-billion-dollar-bets-wisely.pdf)

Mliu92 & Wikimedia Commons. (2021, August 6). CHADeMO Connector. Wikimedia Commons. [https://en.wikipedia.org/wiki/CHAdeMO#/media/File:CHAdeMO_connector.svg](https://en.wikipedia.org/wiki/CHAdeMO#/media/File:CHAdeMO_connector.svg)

Miles, D. (2010). A Brief Outline of J1772 Operation and Configuration. In Electric Vehicle Discussion List. [http://www.evdl.org/docs/j1772description.pdf](http://www.evdl.org/docs/j1772description.pdf)

Nar, S. (2023, August 15). A Tesla parked in front of an EV charging station at Toronto’s Trinity Bellwoods Park gets a charge in October 2021. CBC. [https://i.cbc.ca/1.6935761.1692025430!/cumulusImage/httpImage/image.jpg_gen/derivatives/16x9_780/photos-ev-charging-station.jpg](https://i.cbc.ca/1.6935761.1692025430!/cumulusImage/httpImage/image.jpg_gen/derivatives/16x9_780/photos-ev-charging-station.jpg)

National Renewable Energy Laboratory. (2023). The 2030 National Charging Network: Estimating U.S. Light-Duty demand for electric vehicle charging infrastructure. In nrel.com (NREL/FS-5400-85970). United States Department of Energy. [https://www.nrel.gov/docs/fy23osti/85654.pdf](https://www.nrel.gov/docs/fy23osti/85654.pdf)

Natural Resources Canada [N.R Canada]. (2023, October 27). Electric Vehicle and Alternative Fuel Infrastructure Deployment Initiative. Retrieved March 12, 2024, from [https://natural-resources.canada.ca/energy-efficiency/transportation-alternative-fuels/infrastructure/electric-vehicle-alternative-fuels-infrastructure-deployment-initiative/18352](https://natural-resources.canada.ca/energy-efficiency/transportation-alternative-fuels/infrastructure/electric-vehicle-alternative-fuels-infrastructure-deployment-initiative/18352)

Quick 220 Electrical Systems. (n.d.). North American voltage ranges. [https://quick220.com/pages/north-american-voltage-ranges](https://quick220.com/pages/north-american-voltage-ranges)

Rempel, D., Cullen, C., Bryan, M. M., & Cezar, G. (2022). Reliability of open public electric vehicle direct current fast chargers. Social Science Research Network. [https://doi.org/10.2139/ssrn.4077554](https://doi.org/10.2139/ssrn.4077554)

SAE International. (2021). Sustainable mobility Solutions electric vehicle charging data performance & reporting. In Sustainable Mobility Solutions - SAE International. [https://sms.sae.org/binaries/content/assets/cm/content/sms/cspr-published-document-2023.pdf](https://sms.sae.org/binaries/content/assets/cm/content/sms/cspr-published-document-2023.pdf)

SAE International. (2023, June 28). SAE International announces Standard for NACS connector, charging PKI and infrastructure Reliability. [https://www.sae.org/site/news/press-room/2023/06/sae-international-announces-standard-for-nacs-connector](https://www.sae.org/site/news/press-room/2023/06/sae-international-announces-standard-for-nacs-connector)

Shimizu, R., Kawakami, A., & Yao, T. (2023, October 20). Tesla’s EV chargers win over Toyota, but next test will be Asia. Nikkei Asia. [https://asia.nikkei.com/Business/Automobiles/Tesla-s-EV-chargers-win-over-Toyota-but-next-test-will-be-Asia](https://asia.nikkei.com/Business/Automobiles/Tesla-s-EV-chargers-win-over-Toyota-but-next-test-will-be-Asia)

Statistics Canada. (2024). New motor vehicle registrations, quarterly [Dataset;Web]. In Table 20-10-0024-01. [https://doi.org/10.25318/2010002401-eng](https://doi.org/10.25318/2010002401-eng)

Tesla, Inc. (2022). North American Charging Standard Technical Specification. Tesla Standard Technical Specification Board. [https://tesla-cdn.thron.com/static/HXVNIC_North_American_Charging_Standard_Technical_Specification_TS-0023666_HFTPKZ.pdf?xseo=&response-content-disposition=inline%3Bfilename%3D%22North-American-Charging-Standard-Technical-Specification-TS-0023666.pdf%22](https://tesla-cdn.thron.com/static/HXVNIC_North_American_Charging_Standard_Technical_Specification_TS-0023666_HFTPKZ.pdf?xseo=&response-content-disposition=inline%3Bfilename%3D%22North-American-Charging-Standard-Technical-Specification-TS-0023666.pdf%22)

Tommy84, Undead_Ready, Wojitas_ & Fissionpowered. (2021). Stuck CHAdeMO? [Online forum post]. Reddit. [https://www.reddit.com/r/leaf/comments/o8ptkt/stuck_chademo/](https://www.reddit.com/r/leaf/comments/o8ptkt/stuck_chademo/)

Transport Canada. (2024, January 15). Zero-emission vehicle charging stations. [https://tc.canada.ca/en/road-transportation/innovative-technologies/zero-emission-vehicles/zero-emission-vehicle-charging-stations#/find/nearest?country=CA](https://tc.canada.ca/en/road-transportation/innovative-technologies/zero-emission-vehicles/zero-emission-vehicle-charging-stations#/find/nearest?country=CA)