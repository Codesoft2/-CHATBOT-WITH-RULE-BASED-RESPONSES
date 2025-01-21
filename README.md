def chatbot(user_input):
    user_input = user_input.lower()

    if "hello" in user_input or "hi" in user_input:
        return "Hello! How can I assist you?"
    elif "how are you" in user_input:
        return "I'm just a AI, but thanks for asking! How can I help you?"
    elif "what is your name" in user_input:
        return "You can call me Chatbot!"
    elif "help" in user_input:
        return "Sure! What do you need help with?"
    elif "bye" in user_input or "exit" in user_input:
        return "Goodbye! Have a great day!"
    else:
        return "I'm sorry,I didn't understand that.Can you please repeat it?"

def main():
    print("Welcome to the chatbot!")
    while True:
        user_input = input("You: ")
        if user_input.lower() in ["exit", "bye"]:
            print("Chatbot: Goodbye! Have a great day!")
            break
        response = chatbot(user_input)
        print("Chatbot:", response)

if __name__ == "__main__":
    main()




