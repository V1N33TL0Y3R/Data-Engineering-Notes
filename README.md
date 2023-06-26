# Data-Engineering
Data Engineering notes

## What is the Data Flow?
#### Data Flow contains 4 primary stages 
    1. Data Collection and Storage
    2. Data Preparation
    3. Exploration and Visualization
    4. Experimentation and Prediction

## Role of Data Engineers?
Data Engineers are responsible for the first stage of Data Flow i.e. Data Collection and Storage
They have a great responsibility as they lay the ground work for data analysts, data scientists and ML engineers. If the data is scattered around, corrupted and difficult to access, there's not much to prepare, explore or experiment with. 

-> Data Engineers develop, construct, test and maintain architectures such as databases and large scale processing systems to process and handle massive amounts of data.

## Classifying data 
#### The five V's - 
  1. Volume ( quantity of data points ) 
  2. Variety ( type and nature of the data: text, image, audio, video etc. )
  3. Velocity ( how fast the data is generated and processed )
  4. Veracity ( how trustworthy the sources are )
  5. Value ( how actionable the data is )


## Data Engineers vs Data Scientists 

Data Engineers works on first phase of Data Flow - Data Collection and Storage 
Data Scientists works on the rest of the phases - Data Prep, Exploration and Visualization, Experimentation and Prediction.
Example -  person collectes and stores customer, artists, song data in their respective DB -> Data Engineer 
           person uses the collected data to understand the listening pattern or build recommendation engines -> Data Scientists


## The Data Pipeline

Imagine an oil pipeline -> you extract crude oil from oil fields then move it to distillation unit through pipeline -> seperate residue -> heavy oil -> diesel -> Kerosene -> Napththa -> Gasoline and each of the product have a seperate pipeline. Say Kerosene is transported to airports, Gasoline is trasported to several petrol stations etc etc.
Similarly, data is the new oil !!

Companies ingest data and it needs to be processed and stored in various ways. To handle the data we need data pipelines that efficiently automates the flow from one station to the next, so that data scientists can use up-to-date, accurate info. 

Ex. A music company collects data of users through their mobile app, desktop and web app.(3 pipelines) -> the data is collected into [ DataLake ] -> now we can have multiple DBs such as employees, customer, playlists, tracks, albums, artists (6 pipelines) -> furthermore, say employees are from US,UK,IN (3 pipelines) -> albums can have multiple pictures (2 pipelines)....so on

<img width="647" alt="image" src="https://github.com/Ony-mous/Data-Engineering-/assets/30760868/b550485f-899d-42fc-aea8-a92d05e71191">


Functions of a Data Pipeline is to automate : Extracting, Transforming, Validating, Combining, Loading data.

Difference between ETL and Data pipeline -> ETL is a popular framework for designing data pipelines, data is processed before it is stored. One may or may not follow ETL ex. data is given directly after extracting to visualization tools rather than transforming.


Requirement -> need to give recommended songs list to our user 

Data Flow ->  
1. extract songs our user listned the most over the last 2-3 months. <br>
2. Find other users who listned to same song.<br>
3. Extract songs from these users listning history -"similar profile"<br>
4. extract songs from the above steps which belong to same genre as the one which our user listnes to.<br>
5. These songs will be our "recommendation". <br>


           
