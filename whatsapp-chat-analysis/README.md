This is a Streamlit-based web application that analyzes WhatsApp chat data to provide insights and visualizations about message activity, user behavior, and overall communication trends in a chat. The application processes exported WhatsApp chat files in .txt format and provides a user-friendly interface to explore statistics, timelines, and more.

Features

1. Upload Chat File

Users can upload their exported WhatsApp chat file (in .txt format).

The application preprocesses the data for analysis.

2. User Selection

Analyze data for individual users or for the entire group.

Excludes "group_notification" messages.

3. Key Statistics

Displays the following statistics for the selected user or group:

Total Messages

Total Words

Media Shared

Links Shared

4. Timelines

Monthly Timeline: View message activity over months.

Daily Timeline: Observe message activity on a daily basis.

5. Activity Maps

Most Busy Day: Analyze activity trends by days of the week.

Most Busy Month: Identify activity by months.

Weekly Activity Heatmap: Visualize user activity across hours and days of the week.

6. Busiest Users (Group-level analysis)

Identify the most active users in the group.

Displays data as both a bar chart and a table.

7. WordCloud

Generates a WordCloud for the most frequently used words.

8. Most Common Words

Displays the most common words used in the chat as a horizontal bar chart.

9. Emoji Analysis

Provides insights into emoji usage:

Emoji counts displayed in a table.

Pie chart for the top 5 most-used emojis.

How to Use

Prerequisites

Install Python (>= 3.8).

Install required libraries using the following command:

pip install streamlit matplotlib seaborn

Running the Application

Clone the repository or copy the code to your local machine.

Save the preprocessor.py and helper.py files in the same directory as the main script.

Open a terminal and navigate to the directory containing the script.

Run the following command to launch the application:

streamlit run app.py

Upload your WhatsApp .txt file via the sidebar.

Select a user or analyze the entire chat.

Explore the insights and visualizations provided.

File Descriptions

1. app.py

Main script to run the Streamlit application. Contains the logic for user interface and integration with helper functions.

2. preprocessor.py

Contains functions for preprocessing the uploaded WhatsApp chat data, including:

Parsing dates and times.

Extracting user messages.

3. helper.py

Contains utility functions for generating insights and visualizations, such as:

Fetching statistics.

Generating timelines.

Creating WordClouds.

Emoji analysis.

Sample Data

Ensure the WhatsApp chat file is exported in .txt format. Example of the file format:

12/01/2023, 9:15 PM - John: Hello everyone!
12/01/2023, 9:16 PM - Jane: Hi John!

Dependencies

Python (>= 3.8)

Streamlit

Matplotlib

Seaborn

Pandas

WordCloud

Install dependencies using:
