# Task1

**Build a simple chatbot that responds to user inputs based on
predefined rules. Use if-else statements or pattern matching
techniques to identify user queries and provide appropriate
responses.**

import java.util.Scanner;

public class ChatBot {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Hello! I'm ChatBot. Type 'exit' to end the conversation.");
        
        while (true) {
            System.out.print("You: ");
            String userInput = scanner.nextLine().toLowerCase();
            
            if (userInput.equals("exit")) {
                System.out.println("ChatBot: Goodbye! Have a wonderful day!");
                break;
            } else if (userInput.contains("hello") || userInput.contains("hi")) {
                System.out.println("ChatBot: Hi there! How can I assist you today?");
            } else if (userInput.contains("how are you")) {
                System.out.println("ChatBot: I'm a bot, so I don't have feelings, but I'm here to help!");
            } else if (userInput.contains("your name")) {
                System.out.println("ChatBot: I'm ChatBot, your virtual assistant.");
            } else if (userInput.contains("help")) {
                System.out.println("ChatBot: Of course! What do you need help with?");
            } else if (userInput.contains("weather")) {
                System.out.println("ChatBot: I can't check the weather right now, but you can try a weather website!");
            } else {
                System.out.println("ChatBot: Sorry, I didn't understand that. Could you rephrase?");
            }
        }
        
        scanner.close();
    }
}
