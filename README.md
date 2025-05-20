# API-INTEGRATION-AND-DATA-VISUALIZATION

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: SHREYKUMAR SANDIPKUMAR PATEL

*INTERN ID*: CT04DL1307

*DOMAIN*: PYTHON PROGRAMMING

*DURATION*: 4 WEEKS 

*MENTOR*: NEELA SANTOSH

*DESCRIPTION*:
                 Task 1: API Integration and Data Visualization Using Python
As part of my Python internship under CodTech, Task 1 involved integrating a public API into a Python project and creating visualizations based on the data retrieved. I selected the OpenWeatherMap API, a widely used service that provides real-time and forecasted weather data. The objective was to fetch weather forecast data for a specific city and then visualize the temperature trends using libraries like Matplotlib and Seaborn.
Project Overview and Setup
To begin, I imported all the necessary Python libraries including requests for making API calls, json for handling JSON data, pandas for data manipulation, and matplotlib.pyplot and seaborn for data visualization. I obtained a free API key from the OpenWeatherMap platform and used it to construct an HTTP GET request URL for fetching forecast data for the city of Mumbai. The API call returned a JSON response containing detailed weather forecasts in 3-hour intervals over a 5-day period.

I ensured robust error handling by checking the status code of the response and verifying that the key 'list' existed in the returned JSON data. If the API returned an error or the expected structure was missing, the script would print a clear message, preventing runtime errors or crashes.
Data Extraction and Processing
Once the API response was verified, I parsed the JSON to extract relevant fields. Specifically, I focused on the forecast timestamps (dt_txt) and corresponding temperature readings (temp). I stored these values in two separate lists—times and temps. This step involved iterating over the JSON structure and accessing nested dictionaries within the forecast data.

After collecting the necessary data, I created a Pandas DataFrame to organize the extracted data into a tabular format. This not only made the data easier to manage but also facilitated seamless integration with visualization libraries. For clarity and focus, I limited the dataset to the first 10 records, which represent a series of short-term forecasts.
Data Visualization
With the DataFrame prepared, I moved on to creating a visual representation of the temperature trend. I used Seaborn's lineplot to graph temperature against time, providing a clear visual of how the temperature is expected to change in Mumbai over the forecasted period. To improve readability, I rotated the x-axis labels, added axis labels, a title, and enabled grid lines using Matplotlib functions.

The resulting plot offered a concise yet informative look at weather dynamics over time, allowing viewers to grasp changes in temperature at a glance.
