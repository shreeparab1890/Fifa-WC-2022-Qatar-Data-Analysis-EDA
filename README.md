# Fifa WC 2022 Qatar Data Analysis EDA
This ipython notebook is the <b>Exploratory data analysis (EDA)</b> of the <b>FIFA WC Qatar 2022</b>. 
The dataset used has been compiled from various sources by web scrapping. 
You can follow the analysis on <a href="https://www.kaggle.com/code/shrikrishnaparab/fifa-wc-2022-qatar-data-analysis-eda">kaggle</a>

![FIFA WC 2022 Qatar](dataset-cover.jpg)

## Python Packeges Used:
**Numpy, Pandas, Matplotlib, Seaborn, Plotly**

# What is Exploratory Data Analysis?
Exploratory Data Analysis (EDA) is a technique used to gain insights and understanding from a given dataset. It is an approach for analyzing and summarizing data that allows analysts to identify patterns, trends, and relationships within the data. EDA is typically the first step in the data analysis process and also is an iterative process that involves visualizing and summarizing the data in various ways.

The main goal of EDA is to develop a deeper understanding of the data and identify any potential issue or limitation. This process allows analysts to clean and prepare the data for further analysis, and can also reveal insights that can guide the analysis to move in a proper direction.

One of the key tools used in EDA is visualization. Visualizing data in various ways can reveal patterns and relationships that may not be immediately apparent when looking at raw data.  
Common visualizations used in EDA include:
  1. Histograms
  2. Scatter plots
  3. Box Plots
  4. Bar Charts
  5. Line Charts
  6. Pie Chart or Donut Chart
  7. Bubble Charts  
These visualizations can be used to identify outliers, patterns, and trends in the data, and can also be used to compare different subsets of the data.

Another important aspect of EDA is summarizing the data using statistical measures such as mean, median, standard deviation nd plotting the Corelation Matrix. These measures can be used to understand the distribution of the data and identify any potential outliers.

EDA can also include data cleaning and preprocessing, which is the process of identifying and correcting errors or inconsistencies in the data. This can include handling missing data, removing outliers, or transforming variables to make the data more suitable for analysis.

Overall, EDA is a crucial step in the data analysis process, as it allows analysts to gain a deeper understanding of the data and identify any potential issues or limitations before proceeding with more advanced analysis. It also can also be a great way to find the insights that can guide the further analysis.

## Coming Back to the project:  
### Data Collection:
The technique used for data collection is web scrapping and data is compiled in a CSV file. The CSV file consist of 59 Columns and has data of all 64 matches played in the world cup 2022. 
The columns can be divided into:
### Basic Match details: 
  - match_no	
  - day_of_week	
  - date	
  - hour	
  - venue	
  - referee	
  - group	
  - 1	(Team 1)
  - 2	(Team 2)
  - attendance
### Other Details: (which are used in the EDA)
  - 1_xg	
  - 2_xg	
  - 1_poss	(Team 1 Possesion) 
  - 2_poss	(Team 2 Possesion) 
  - 1_goals	(Team 1 Goal Scored) 
  - 2_goals	(Team 2 Goal Scored) 
  - score (Fianl Scored of the match)
  - 1_yellow_cards	(Team 1 Yellow Cards)
  - 2_yellow_cards	(Team 2 Yellow Cards)
  - 1_red_cards	(Team 1 Red Cards)
  - 2_red_cards	(Team 2 Red Cards)
  - 1_passes	(Team 1 Passes)
  - 2_passes	(Team 2 Passes)
  - 1_passes_compeletd	(Team 1 Passes completed)
  - 2_passes_compeletd  (Team 2 Passes completed)
  - 1_own_goal	(Own Goal by Team 1)
  - 2_own_goal	(Own Goal by Team 2)

For Analysis purpose we have done feature engineering on the above csv file to create new columns(Features):
1. Total Match Goals ( we have added 1_goals and 2_goals)
2. Pass Acuracy ( (1_passes / 1_passes_compeletd)*100)

The Dataset(CSV) does not have any null data and has no duplicate entry. 




