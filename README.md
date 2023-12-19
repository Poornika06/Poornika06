 chatbot using conditional statements and loops in Python:

python
import random

print("Welcome to the Chatbot!")

while True:
    user_input = input("You: ").lower()

    if "hello" in user_input:
        print("Chatbot: Hi there! What's on your mind?")
    elif "how are you" in user_input:
        print("Chatbot: I'm doing well, thank you! How about you?")
    elif "bye" in user_input or "exit" in user_input:
        print("Chatbot: Goodbye! Have a fantastic day!")
        break
    elif "tell me a fact" in user_input:
        facts = ["The honeybee is the only insect that produces food eaten by humans.", 
                 "The Great Wall of China is the longest wall in the world.",
                 "Bananas are berries, but strawberries aren't."]
        random_fact = random.choice(facts)
        print(f"Chatbot: Here's a fact for you - {random_fact}")
    elif "favorite color" in user_input:
        colors = ["Blue", "Green", "Red", "Purple", "Yellow"]
        favorite_color = random.choice(colors)
        print(f"Chatbot: My favorite color is {favorite_color}. What's yours?")
    else:
        print("Chatbot: I'm not sure how to respond to that. Feel free to ask something else or type 'bye' to exit.")


This chatbot responds to greetings, inquires about its well-being, shares random facts, talks about its favorite color, and allows the user to exit. Feel free to add more features or modify the responses as per your preferences!
