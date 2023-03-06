# The public version of the quiz bot
- this repo will be updated when there are new things to share

## How to run

### Create a Quiz

- create a new folder in resources folder
- add quiz.txt
- add images

#### quiz.txt

##### Format

The quiz.txt has to be in the following format:
Start Message
End Message
Question1;Answer1;Hint1.1;Hint1.2;Hint1.3;MaxGuesses1
Question2;Answer2;Hint2.1;Hint2.2;Hint2.3;MaxGuesses2

##### Question

- Question: text -> the question
- Answer: text -> the correct answer to the question and how it should ne written
- Hints: text -> the hints to help a player with the question
- MaxGuesses: number -> the amount of wrong guesses a player has between hints. MaxGuesses > 0

##### Special-Charackters

; can not be used as a charackter in a line with a question
| is used to generate a new line in the start/end message

#### images

- has to be .png
- format has to be sendX.png

##### What Number for which picture?

This is fairly simple. To send a picture for question 1 you add the send1.png file, which will then be sent with the question.
So the number is the number of the question, which can be seen on the left hand side in most text editors.

### Run the bot

#### creds.py

- bot token is the token you use to run your discord bot
- folder is the folder where your quiz folder is located 'resources\\your_folder'
- quiz_master_id is the id of the player who manages the quiz (to get an id enable developer mode in discord, then right click -> copy id)
- quiz_channel_id is the channel id where the question will be posted
- table_channel_id is the channel id where the table will be frequently updated (choose a different channel then quiz_channel_id)
- log_channel_id is the channel id where all user answers and hints will be sent to if the question is finished (this shouldnt be the same as table but can be the same as quiz)


#### start the quiz

- you can now start the main.py file, if you get an error open a terminal in the folder and type `pip install discord`
- now if the bot is running you can do /help to see all your commands
- /start -> starts the quiz beginning with the start message (24h later the first question will be sent)
- /start_at number -> starts the quiz at the number e.g. /start_at 3 would instantly sent question number 3 and the next one 24h later
- the quiz should now be running until it is over or you close the main.py


