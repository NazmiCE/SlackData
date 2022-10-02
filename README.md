# SlackData
The goal here was to convert JSON format of Slack Data from a channel to multiple CSV files.
In the directory there are 38 files in a JSON format, and I have iterated each files and extract
the data from them, and I have created 4 csv files.

The first one is user_info.csv which contains user_id and real name.
The second one is reactions.csv which contains client_message_id, ts (time send in timestamps), name (reaction name) and user id.
The third one is thread.csv which contains client_message_id, ts (time send in timestamps), user (user id) and text.
The fourth and final one is thread_reactions.csv which contains thread_ts, parent_user_id, ts (child), user (child). 

Since we don't have exact threads for each day. Extracting reactions for a spesific day may cause error. To solve this problem
I have used try and catch methods, but by doing that I may lost some information so a better organization should be implemented.
