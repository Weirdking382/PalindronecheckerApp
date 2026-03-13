import java.util.Scanner;

public class PalindromeApp {
public static void main(String[] args) {
Scanner scanner = new Scanner(System.in);

        // Instantiate the object (OOP approach)
        PalindromeService service = new PalindromeService();

        System.out.println("--- UC11: Object-Oriented Palindrome App ---");
        System.out.print("Enter your text: ");
        String userInput = scanner.nextLine();

        // Use the service method
        boolean result = service.checkPalindrome(userInput);

        if (result) {
            System.out.println("Success: This is a palindrome!");
        } else {
            System.out.println("Result: Not a palindrome.");
        }

        scanner.close();
    }
}