# minorproject1
GroupDNA – WhatsApp Group Chat Analysis
📌 Project Overview

GroupDNA is a Python-based WhatsApp group chat analysis project that extracts useful information from an exported WhatsApp chat and generates a detailed analysis of group communication patterns.

The project analyzes the chat to understand:

Group activity
Message contribution of each participant
Most active days and hours
Participant activity by hour
Frequently used words
Average message length
Response patterns
Longest silent streaks
Fun and interesting personality archetypes

The project is implemented using Python and NumPy.

🎯 Objectives

The main objectives of GroupDNA are:

To process and analyze an exported WhatsApp group chat.
To identify the most active participants.
To find the busiest day and busiest hour of the group.
To analyze the activity pattern of each participant.
To identify the most frequently used words.
To calculate the average message length of participants.
To analyze response time between participants.
To identify the longest silent period of each participant.
To classify participants into simple personality archetypes based on their chat behavior.
🛠️ Technologies Used
Python 3
NumPy
Jupyter Notebook / Google Colab
WhatsApp exported chat .txt file
Python Libraries
numpy
datetime
📂 Project Structure
GroupDNA/
│
├── minorproject1.ipynb
├── WhatsApp Chat.txt
└── README.md
📥 Input Dataset

The project uses an exported WhatsApp group chat in .txt format.

The notebook reads the chat file and processes:

Date and time
Sender name/number
Message text
System messages
Media messages
Deleted messages

The current notebook is configured to read:

WhatsApp Chat with Sec A Msec (notes).txt

Update the FILE_NAME variable if a different chat export is used.

⚙️ How the Project Works
1. Read WhatsApp Chat

The program reads the exported WhatsApp text file line by line.

2. Parse Messages

Each message is separated into:

Timestamp
Sender
Message text

The program also handles multi-line messages.

3. Remove Unwanted Messages

The system identifies and separates:

System messages
Media messages
Deleted messages

Only real text messages are used for the main analysis.

4. Convert Date and Time

The timestamp is converted into Python datetime objects so that date and time-based analysis can be performed.

5. Group Overview

The project calculates:

Total number of messages
Number of participants
Chat duration
Messages sent by each participant
Percentage contribution of each participant
6. Activity Analysis

The project identifies:

Busiest day
Busiest hour
Participant activity by hour

An activity heatmap is generated using symbols such as:

.  ░  ▒  █
7. Frequently Used Words

The project removes selected common stop words and calculates the frequency of other words.

The top 10 frequently used words are displayed.

8. Average Message Length

For every participant, the average number of words per message is calculated.

9. Response Pattern Analysis

The project calculates the average time taken by participants to respond when the next message is sent by another participant.

It also identifies:

Fastest replier
Slowest replier
10. Silent Streak Analysis

The project calculates the longest period during which a participant did not send a message.

11. Personality Archetypes

Participants are assigned simple chat-based archetypes using predefined rules.

The project includes:

Spammer
Group Mom
Night Owl
Storyteller
Drama Queen
Ghost
Comedian
Question Master
Regular User

These classifications are based on measurable chat characteristics rather than psychological diagnosis.

📊 Features
Feature	Description
Chat Parsing	Reads and processes WhatsApp exported chat
Message Count	Counts messages from each participant
Group Overview	Displays overall group statistics
Activity Peaks	Finds busiest day and hour
Activity Heatmap	Shows activity by participant and hour
Top Words	Finds frequently used words
Message Length	Calculates average words per message
Response Analysis	Calculates response time
Silent Streak	Finds longest inactive period
Archetype Detection	Assigns chat-based personality categories
📈 Sample Results

The analyzed dataset in the notebook contains:

877 days of chat activity
2361 real messages
71 participants
Chat period from 26 March 2024 to 19 August 2026

The busiest day identified was:

15 May 2025
101 messages

The busiest hour was:

11:00 – 12:00
269 messages

The most frequently occurring words included:

will
class
lab
all
students
your
come
with
group
who

These values are based on the dataset processed in the uploaded notebook.

🚀 Installation

Install Python 3 and NumPy.

pip install numpy

For Jupyter Notebook:

pip install notebook
▶️ Running the Project
Using Jupyter Notebook
Open Jupyter Notebook.
Open minorproject1.ipynb.
Export your WhatsApp group chat as a .txt file.
Place the .txt file in the required location.
Update the FILE_NAME variable in the notebook.
Run all cells.
Using Google Colab
Upload minorproject1.ipynb to Google Colab.
Upload the WhatsApp .txt file.
Update the file path.
Run the notebook cells.
View the generated analysis in the output.
🔒 Privacy

WhatsApp chat data may contain private information such as names, phone numbers, and personal messages.

Therefore:

Do not publicly share the original chat file.
Remove sensitive information before publishing the project.
Use anonymized data for demonstrations and presentations.
Keep the dataset only for authorized analysis.
⚠️ Limitations
The project depends on the format of the exported WhatsApp chat.
Different WhatsApp export formats may require changes to the parser.
Personality archetypes are rule-based and should be considered entertainment-oriented analysis.
Response-time calculations depend on message ordering and timestamps.
The current implementation uses a predefined list of stop words.
The analysis is mainly based on text messages and does not analyze the actual content of media files.
🔮 Future Enhancements

The project can be improved by adding:

Interactive dashboards
Graphical charts
Sentiment analysis
Emoji analysis
Monthly and yearly activity trends
Topic detection
Word clouds
Advanced NLP techniques
Machine learning-based personality classification
Automatic report generation
Support for multiple WhatsApp export formats
📚 Learning Outcomes

Through this project, we learn how to:

Work with real-world text data
Parse semi-structured data
Use Python for data analysis
Use NumPy for numerical processing
Work with dates and timestamps
Calculate statistical information
Analyze communication patterns
Build rule-based classification systems
👩‍💻 Project Type

Minor Project

Domain

Data Science / Data Analytics / Natural Language Processing

Programming Language

Python

Main Library

NumPy
