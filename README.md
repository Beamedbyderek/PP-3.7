# PP-3.7

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Main.java to edit this template
 */
package pp.pkg3.pkg7;

import java.util.Scanner;

public class PP37 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
       Scanner keyboard = new Scanner(System.in);

		double sideA, sideB, sideC, halfPerimeter;		
		double area;

		System.out.println("The user will enter each length of the triangle's three sides separately.");
                
                System.out.print("length of side A: ");
		sideA = keyboard.nextDouble();
		System.out.print("length of side B: ");
		sideB = keyboard.nextDouble();
		System.out.print("length of side C: ");
		sideC = keyboard.nextDouble();
                
                halfPerimeter = (sideA + sideB + sideC) * 0.5;		// Calculate half of the triangle's perimeter. 

		area = Math.sqrt(halfPerimeter * (halfPerimeter - sideA) * (halfPerimeter - sideB) * (halfPerimeter - sideC));

		System.out.println("The area of the triangle is: " + String.format("%.3f",area));

    }
    
}
