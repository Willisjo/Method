
package java_methods;

import java.util.Scanner;

public class Methods {
    public static void main(String args) {
        int numbers = getNumbersFromUser();
        int smallestNumber = findSmallestNumber(numbers);
        int largestNumber = findLargestNumber(numbers);
        
        displayResults(smallestNumber, largestNumber);
    }
    
    public static int getNumbersFromUser() {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Enter the first number: ");
        int firstNumber = scanner.nextInt();
        
        System.out.print("Enter the second number: ");
        int secondNumber = scanner.nextInt();
        
        System.out.print("Enter the third number: ");
        int thirdNumber = scanner.nextInt();
        
        int numbers = {firstNumber, secondNumber, thirdNumber};
        return numbers;
    }
    
    public static int findSmallestNumber(int numbers) {
        int smallestNumber = numbers[0        
        for (int i = 1; i < numbers.length; i++) {
            if (numbers < smallestNumber) {
                smallestNumber = numbers;
            }
        }
        
        return smallestNumber;
    }
    
    public static int findLargestNumber(int numbers) {
        int largestNumber = numbers[0        
        for (int i = 1; i < numbers.length; i++) {
            if (numbers[i largestNumber) {
                largestNumber = numbers[i            }
        }
        
        return largestNumber;
    }
    
    public static void displayResults(int smallestNumber, int largestNumber) {
        System.out.println("The smallest number: " + smallestNumber);
        System.out.println("The largest number: " + largestNumber);
        System.out.println(smallestNumber + " is your smallest number.");
        System.out.println(largestNumber + " is your largest number.");
    }
}
