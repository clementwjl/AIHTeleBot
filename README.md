# AIHTeleBot

As part of your project, you are required to implement a chatbot using Langchain. However, implementing a whole new web application may be too tedious and out-of-scope, so we have provided code to implement your code to a telegram bot instead!

# What to do: 

## 1. Clone to your repository

On your preferred IDE, open the folder that you wish you put the project in, and proceed to run the following in your shell:

```
git clone https://github.com/zhengfeng-toh/AIHTeleBot
```

And afterwhich,

```
cd AIHTeleBot
```

## 2. Creating the environment variables

On the `aihbot` directory, create a `.env` file or use an existing one (if you have from the lab). The format should be as such:

```
OPENAI_API_KEY=sk-YOUR_OPENAI_APIKEY
LANGSMITH_API_KEY=ls__YOUR_LS_APIKEY
TELEGRAM_BOT_TOKEN=YOUR_BOTTOKEN
```

We will talk about how to get your Telegram bot token in the next step.

## 3. Get your telegram API key

You will need the API key to connect to a bot. This requires you to navigate to [BotFather](https://t.me/BotFather). Do refer to [this video](https://www.youtube.com/watch?v=aNmRNjME6mE&ab_channel=SmartBotsLand) should you need help to gather the API key.

After you receive the API key, save it into the `.env` file.

## 4. Install all dependencies

Windows: 
Run the following on your shell (Command Prompt)

```
pip install -r requirements.txt
```

Mac: Run the following on your shell (zsh)
```
pip3 install -r requirements.txt
```

## 5. How to make your code run with the bot

There are two Python files that will be running the show, `bot.py` and `model.py`.

- `model.py` will be the file that your project is running.

- `bot.py` will assist in receiving and sending out responses. 

Modify `model.py` with your langchain model. You may use helper functions or even change `bot.py` to suit your project requirements. Ultimately, it is up to your group to decide how the chatbot should behave. 

## 6. Test the bot

Time for you to try your very creation!

Windows: Run the following on your shell (Command Prompt)
```
python bot.py
```

Mac: Run the following on your shell (zsh)
```
python3 bot.py
```

If everything works, it should produce the following:
```
Loading configuration...
Successfully loaded! Starting bot...
```

Have fun creating your chatbot!


# Error debugging

My terminal says
```
 File "/opt/homebrew/lib/python3.11/site-packages/chromadb/api/types.py", line 99, in maybe_cast_one_to_many
    if isinstance(target[0], (int, float)):
                  ~~~~~~^^^
IndexError: list index out of range
```

A: Create a folder called docs, add all your relevant documents inside.