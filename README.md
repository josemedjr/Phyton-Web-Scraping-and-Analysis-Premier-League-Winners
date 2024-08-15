## Web Scraping and Data Analysis on Premier League Winning Teams using Python




## Problem Description 
I utilized Beautiful Soup and web scraping techniques in Python to extract data on Premier League winning teams from Wikipedia. After gathering the data, I employed Pandas to structure it into a table and performed data cleaning to enhance its usability. Following this, I conducted a comprehensive analysis and developed visualizations to identify patterns and similarities among the winning teams, focusing on metrics such as goals scored, goals against, wins, losses, and other relevant factors.



## Web Scraping
I began the project by importing BeautifulSoup and printing the webpage I intended to scrape. Using the find_all function, I located the specific table on the page that contained the data I needed. To extract the column titles, I employed find_all for the 'th' tags, while tr was used to retrieve each row of the dataset. To refine the data, I applied text.strip() to clean the text elements. Once the data was properly extracted and cleaned, I imported Pandas to organize the columns and raw data into a structured table, which I then convereted into a CSV file. 

## Data Cleaning and Analysis
Once the table was created using Pandas, I began the process of cleaning the data to ensure its usefulness. I started by dropping columns that were not relevant to the analysis. To better understand the dataset, I used df.info() to check the data types of each column. Since all columns were initially identified as objects, I needed to convert certain columns to numerical data types. To do this, I applied pd.to_numeric, converting the necessary columns to floats (e.g., df['Played'] = pd.to_numeric(df['Played'], errors='coerce')). After the data was properly cleaned and organized, I moved on to the analysis phase by grouping the data based on the "Winners." I transposed the DataFrame to facilitate accurate and efficient visualization, allowing me to employ various visualization techniques such as plots, bar graphs, and pie charts. These visualizations helped in analyzing the teams' performance metrics, including wins, losses, points, and more.






