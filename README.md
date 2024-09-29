# random-projects

# iMessage Query with ollama

## Overview
This script allows you to query and analyze your iMessage conversations on macOS using natural language processing.

## Features
- Search for messages from specific senders
- Retrieve full conversations
- Analyze and summarize conversation content
- Use natural language queries to interact with your iMessage data

## Dependencies
- Python 3.12
- langchain
- langchain-openai
- langchain-ollama
- langgraph
- sqlite3
- IPython (for Jupyter Notebook usage)

## Important Setup Step
Before running the script, you must grant Full Disk Access to the application you'll be using to run the Python script (e.g., VS Code, Terminal, or any other IDE). This is crucial for accessing the iMessage database.

To grant Full Disk Access:
1. Open System Preferences > Privacy & Security > Full Disk Access
2. Click the lock icon to make changes (you may need to enter your password)
3. Click the '+' button to add an application
4. Navigate to and select your preferred Python IDE or Terminal app
5. Ensure the checkbox next to the added application is ticked

Without this step, the script won't be able to access your iMessage data.

## Installation
1. Make sure you have Python 3.12 installed on your system.
2. Install the required packages:
   ```
   pip install langchain langchain-openai langchain-ollama langgraph
   ```

## Usage
1. Run the script in a Jupyter Notebook or as a Python script.
2. Input natural language queries to search for and analyze your iMessage conversations.

## Important Notes
- The default path for the iMessage database is `~/Library/Messages/chat.db`. Update the `imessage_db_path` variable if yours is different.
- The script uses a local language model (`llama3.2:3b-instruct-fp16`). Make sure you have this or replace it with a compatible model.

## Privacy and Security
- This script accesses your personal message data. Use it responsibly.
- Don't share the output if it contains personal or sensitive information.

## Limitations
- This script is designed for macOS only.
- Performance may vary based on your iMessage database size and machine capabilities.

## Troubleshooting
- If you get permission errors, double-check the Full Disk Access settings.
- For language model issues, refer to the Ollama documentation.

Enjoy exploring your iMessage data!
