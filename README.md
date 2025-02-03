# Task1

**Build a simple chatbot that responds to user inputs based on
predefined rules. Use if-else statements or pattern matching
techniques to identify user queries and provide appropriate
responses.**

import java.util.Scanner;

public class SimpleChatbot {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Hello! I'm a simple chatbot. Type 'bye' to exit.");
        
        while (true) {
            System.out.print("You: ");
            String userInput = scanner.nextLine().toLowerCase();
            
            if (userInput.contains("hello") || userInput.contains("hi")) {
                System.out.println("Chatbot: Hello! How can I help you today?");
            } else if (userInput.contains("how are you")) {
                System.out.println("Chatbot: I'm just a bot, but I'm doing great! How about you?");
            } else if (userInput.contains("your name")) {
                System.out.println("Chatbot: I'm a simple chatbot created in Java!");
            } else if (userInput.contains("bye")) {
                System.out.println("Chatbot: Goodbye! Have a great day!");
                break;
            } else {
                System.out.println("Chatbot: I'm sorry, I don't understand that.");
            }
        }
        
        scanner.close();
    }
}

