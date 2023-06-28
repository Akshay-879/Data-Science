# EDA and Visualizations on Covid-19 clinical trials.

## Description: 

This project focuses on exploring and analyzing clinical trials related to COVID-19. The dataset used in this project contains information about various clinical trials, including their titles, statuses, conditions, interventions, outcome measures, sponsors, and more.

The project begins by importing the necessary libraries, such as NumPy, Pandas, Matplotlib, Seaborn, and NLTK, to handle and visualize the data. Additionally, the project suppresses warnings to ensure a clean output.

Next, the project loads the data from a CSV file into a Pandas DataFrame for further analysis. The DataFrame consists of 5783 rows and 27 columns, representing different variables related to clinical trials.

To gain an initial understanding of the data, the project displays the first few rows of the DataFrame using the head() function. This provides a glimpse of the data structure and the information stored in each column.

The project then examines the data further by calling the info() function on the DataFrame. This displays a summary of the columns, including their names, data types, and the number of non-null values. It shows that most columns contain object (string) data types, while the "Enrollment" column has a float64 data type. The summary also reveals the presence of null values in several columns.

To analyze the null values, the project creates a new DataFrame called "Null_Values." It populates this DataFrame with the names of the columns from the original DataFrame and computes the count of null values and unique values for each column. The resulting DataFrame is displayed with a gradient color scheme highlighting the null count.

Moving on, the project focuses on exploring the research status of the clinical trials. It creates a summary DataFrame called "trial_summary," which counts the occurrences of each research status and calculates the corresponding percentage. The summary is then displayed, indicating the distribution of research statuses. Additionally, a bar plot is generated using Seaborn's catplot() function to visualize the distribution.

The project further investigates the research conditions by generating a word cloud. It converts the text in the "Conditions" column to lowercase and concatenates all the text into a single string. Using the WordCloud library, a word cloud visualization is created, representing the most common keywords found in the "Conditions" column.

The study results are examined next. The project counts the occurrences of different study results, indicating whether results are available or not. The counts reveal that the majority of the trials (5747 out of 5783) have no results available. A countplot is generated to visualize the distribution of study results.

The project then focuses on the sponsors of the clinical trials. It creates a DataFrame called "top_10_sponsors" to count the occurrences of each sponsor and selects the top 10 sponsors with the highest counts. A bar plot is generated to visualize the distribution of sponsors.

Finally, the project explores the demographic aspects of the clinical trials. It analyzes the age and gender distributions of the participants. The "Age" column is processed by removing parentheses and converting all text to lowercase. The processed "Age" column is then counted to determine the distribution of age ranges. The "Gender" column is also counted to determine the distribution of genders. A pie chart is generated to visualize the gender distribution.

Overall, this project provides insights into the characteristics and status of COVID-19 clinical trials. The analysis covers research status, conditions, study results, sponsors, and demographic aspects. The visualizations and findings can be utilized for educational purposes, research, and decision-making in the field of clinical trials.

### Programing Language: 
1. Python

### Libraries:
1. Numpy
2. Pandas
3. Plotly
4. Matplotlib
5. Seaborn
6. Nltk
