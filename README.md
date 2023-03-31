# Quiz Bot

## How to use the bot
- Fork this repository
- Create a Folder in the ressources folder
- Edit the creds.py file with the correct information
- start the main.py and only close it when the bot is finished
- the quiz master has now access to all commands to start the quit, change time etc...

## The Structure of the Folder
There has to be a quiz.txt file with the following format.
```
This is the start message;This is still the start message but a new line.
This is the end message;This is still the end message but a new line.
Category;Question;Answer;Hint1;Hint2;Hint3;Amount of guesses (has to be a number)
Category;Question;Answer;Hint1;Hint2;Hint3;Amount of guesses (has to be a number)
Category;Question;Answer;Hint1;Hint2;Hint3;Amount of guesses (has to be a number)
 .
 .
 .
```

You can add one picture for a question, the picture must namend sendX.png where X is the number of the question.
