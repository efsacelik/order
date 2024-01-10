# order
Orders 3 numbers from great one to little one. 
package patikaAcademy;

import java.util.Scanner;

public class order {

	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);

		int a, b, c;

		System.out.println("Enter the first number:");
		a = scanner.nextInt();

		System.out.println("Enter the second number:");
		b = scanner.nextInt();

		System.out.println("Enter the third number:");
		c = scanner.nextInt();

		if (a > b && a > c) {
			if (b > c) {
				System.out.println("Order is  " + a+ ">" +b+ ">"+c);
			} else {
				System.out.println("Order is   " + a+ ">" +c+ ">"+b);
			}
		} else if (b > a && b > c) {
               if(a>c) {
                	  System.out.println("Order is  " + b+ ">" +a+ ">"+c);
              }else {
                	  System.out.println("Order is  " + b+ ">" +c+ ">"+a);
                  }
        } else if (c>a && c>b) {
        	 if (b>a) {
        	System.out.println("Order is   " + c+ ">" +b+ ">"+a);
        	 }else {
        		 System.out.println("Order is " + c+ ">" +a+ ">"+c);
        	 }
        }
	}

}
