Authors: David Lin and Wilson Tang
Group Name: DJLT

Accounts: Using SQLite3
Passwords hashed with appended salt.

Server:
1) Polls and cccepts all incoming requests
2) validates messages to follow proper protocol sequence.
3) Depending on message type: spawns new thread to log in user, retrieves currently logged in users,
starts a chat session between two users, etc.
4) Writes to log file.

LogViewer:
1) Accesses the logs and displays it with auxiliary functions such as sorting.

Client:
1) Connects the server, sending messages in the expected protocol formats and sequences.
2) Spawns xterm chat window if another user initiates chat with this user while logged in.
3) Requests server for logged in users that is possible to initiate a chat with.
