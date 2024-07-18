# Simple-rule-based-chat-box
def chatbot():
    # Define the rules and responses
    rules = {
        "hi": "Hello! How can I assist you today?",
        "hello": "Hi there! How can I help you?",
        "how are you?": "I'm just a bot, but I'm here to help you!",
        "what is your name?": "I am a simple rule-based chatbot created by a Python script.",
        "bye": "Goodbye! Have a nice day!",
        "thanks": "You're welcome! If you have any other questions, feel free to ask.",
        "help": "I am here to answer your questions. Try asking me something!"
    }
    
    # Function to generate a response based on user input
    def get_response(user_input):
        return rules.get(user_input.lower(), "I'm not sure how to respond to that. Can you ask something else?")
    
    # Main loop to interact with the user
    print("Chatbot: Hi! I am a simple rule-based chatbot. Type 'bye' to exit.")
    while True:
        user_input = input("You: ")
        if user_input.lower() == "bye":
            print("Chatbot: Goodbye! Have a nice day!")
            break
        response = get_response(user_input)
        print(f"Chatbot: {response}")

# Run the chatbot
if _name_ == "_main_":
    chatbot()
