# Home-Work3.5
package com.company;

import javax.crypto.spec.PSource;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        int sum = add(5, 5);
        System.out.println(sum);
        thirdAngleOfTriangle(50, 50);
        year(1973);
        primeNumberCheck(8);
        checkType(138625);
        checkLargest(20.256f, 20.257f, 20.05f);
        vowelOrConsonent('i');

// DOUBT TO PRINT A-Z : DIDNT USE ASCII values
        char c;

        for(c = 'A'; c <= 'Z'; ++c)
            System.out.print(c + " ");
//    Print numbers 1 to 10
//        for (int i = 1; i <= 10; i++) {
//
//            System.out.println("Numbers " + i);
//
//        }
//    Print squares of numbers 1 to 10
//        for (int i = 1; i <= 10; i++) {
//            System.out.println("Squares " + i * i);
//        }
//
//        int a=5,b=6, c=7;
//        System.out.println(a+b+c);
    }

    //    Method to return Sum of three numbers     QUESTION 1
//    input= 3 variables
//    output= 1 variable
//    logic= returning sum
    public static int add(int num1, int num2) {
        return num1 + num2;
    }

    //    int ang1 = 70, ang2 = 50, ang3;               QUESTION 2
//    int total = 180;
//      input= 2 variables
////    output= 1 variable
////    logic= 180- (sum of 2 angles)
    static void thirdAngleOfTriangle(int ang1, int ang2) {
        System.out.println(180 - (ang1 + ang2));

    }

//    Find if year is a leap year.              QUESTION 3
//    input= 1 variable
//    output= Leap or not
//    Logic: ELSE IF: evenly divisble by 4 and NOT by 100, IF: but divisble by 400 then it is a leap year

    static void year(int year) {
        if (year % 400 == 0) {
            System.out.println("This year is a leap year");
        } else if (year % 4 == 0 && year % 100 != 0) {
            System.out.println("This year is a leap year");
        } else {
            System.out.println("This year is not a leap year");
        }
    }


    //    Java Program to check whether input character is vowel or consonant. Word eg: d   QUESTION 4 (ISSUE)
//    input= alphabet(S)
//    output= 2 variables
//    Logic=if alphabet is vowel or consonant
//
    static void vowelOrConsonent(char alphabet) {
        if (alphabet == 'a' || alphabet == 'e' || alphabet == 'i' || alphabet == 'o' || alphabet == 'u') {
            System.out.println("It is a vowel");
        } else {
            System.out.println("It is a consonent");
        }

    }

    //    write to check if its a prime number              QUESTION 5
    static void primeNumberCheck(int number) {
        if (number % 2 != 0) {
            System.out.println("It is a prime number");
        } else {
            System.out.println("It is not a prime number");
        }
    }
// Write a program to find out factorial of a number

    //    Check whether a number if even or odd         QUESTION 6
    static void checkType(int number) {
        if (number % 2 == 0) {
            System.out.println("even number");
        } else {
            System.out.println("odd number");
        }
    }
// Check largest among three numbers    QUESTION 7: NUMBER 3 is not working - DOUBT
//    input = 3 variables
//    output= 1 variable
//    logic= check largest number out of 3

    static void checkLargest(float number1, float number2, float number3) {
        if (number1 > number2 && number1 > number3) {
            System.out.println("Number 1 is greater");
        } else if (number2 > number1 && number2 > number3) {
            System.out.println("Number 2 is greater");
        } else {
            System.out.println("Number 3 is greater");
        }
    }
//    Display alphabets from A to Z using loops(Hint: ASCII values)
//    input= ASCII values
//    output= alphabets A-Z
//    logic= using ASCII values to print alphabets


    }