# Data_cleaning-----Visualization-
 A Deep Dive into Data Cleaning and Visualization using Python 📊


📌 Exploratory Data Analysis:

🖊 To start, I used the head() function to get a quick glimpse of the dataset, which provided essential initial insights into its structure and content.

🖊Identifying missing data is a crucial step, and I used isnull().sum() to count the number of missing values in each column. I also made use of the missing_values parameter to account for various representations of missing data like "N/a," "NAN," and "na."

🖊Visualizing missing data with a heatmap using Seaborn's sns.heatmap() was enlightening. The heatmap allowed me to quickly identify which columns had the most missing data.

🖊To handle missing data, I employed a variety of techniques, including dropna, ffill, bfill, and interpolate. These methods were invaluable in maintaining data integrity while addressing the absence of information.

🖊Filling missing values in specific columns was a precise task, and I used the fillna() function to specify default values, such as '8888' for the 'Cabin' column and '888' for the 'Age' column.

📌 Data Duplication and Cleaning:

🖊 Ensuring that the dataset is free from duplicates is vital, as it can skew analysis. I used duplicated().sum() to count and remove any duplicated rows, thereby enhancing data quality.

📌 Data Visualization for Insights:

🖊Histogram of Age Distribution: The plt.hist() function creates a histogram of passenger ages, dividing them into 20 bins. It provides insights into the age distribution within the dataset, with a specified title and figure size.

🖊Filtering Survived Passengers: You filter the data to create a subset of passengers who have survived using survived_passengers = merged_data[merged_data['Survived'] == 1].

Histogram for Survived Passengers: The second histogram specifically visualizes the ages of passengers who survived, also with 20 bins. It helps identify age-related patterns among survivors.

🖊Axis Labels: You label the x-axis as 'Age' and the y-axis as 'Number of Survived Passengers' to provide context to the viewer.

🖊Title for Visualization: You set a clear title, 'Histogram of Ages for Survived Passengers,' to describe the content of the plot.

🖊Displaying the Plots: The plt.show
() command is used to display both histograms, making them available for analysis and interpretation.
