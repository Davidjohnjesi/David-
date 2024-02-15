# David-
# Importing required libraries
import random

# Define some responses
responses = {
    "hi": ["Hello!", "Hi there!", "Hey!"],
    "how are you": ["I'm doing well, thanks for asking!", "I'm good, how about you?"],
    "what's your name": ["I'm just a humble AI.", "You can call me ChatGPT."],
    "bye": ["Goodbye!", "See you later!", "Bye!"]
}

# Define a function to handle user input
def chat():
    print("Hi! I'm a simple AI. You can chat with me. Type 'bye' to exit.")
    while True:
        user_input = input("You: ").lower()
        if user_input == 'bye':
            print(random.choice(responses["bye"]))
            break
        elif user_input in responses:
            print(random.choice(responses[user_input]))
        else:
            print("I'm not sure how to respond to that.")

# Start the conversation
chat()
