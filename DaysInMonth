/*
 * CSC-239 JAVA
 * Project Name: DaysInMonth
 * Student: Weiquan Mai
 * Date: February 5, 2025
 * Description: This project prompts user to enter the month and year, and
 * displays the month name, year, and number of days in the month
 */

import java.util.Scanner;

public class LeapYear{
    public static void main(String[] args){
    // Create a scanner
    Scanner input = new Scanner(System.in);

    // Array for month names
    String[] month = {"January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"};

    // Prompt user to enter the month and year
    System.out.print ("Enter a month in the year (e.g., 1 for Jan): ");
    int monthNumber = input.nextInt();

    System.out.print ("Enter a year: ");
    int year = input.nextInt();

    // Determine if year is leap year
    boolean isLeapYear = (year % 4 == 0 && year % 100 != 0) || (year % 400 == 0);

    // Determine the number of days in the month
    int days = 0;
    switch (monthNumber){
        case 1 : case 3 : case 5: case 7: case 8: case 10: case 12:
        days = 31;
        break;
        case 4: case 6: case 9: case 11:
        days = 30;
        break;
        case 2:
            if(isLeapYear){
                days = 29;
            } else{
                days=28;
            }
    }
    // Display the result
    System.out.print(month[monthNumber-1] + " " + year + " has " + days + " days");
    
    // Close the scanner
    input.close();

    }
}
