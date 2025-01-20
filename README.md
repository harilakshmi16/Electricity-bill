# Electricity-bill
Electricity Bill

import java.util.Scanner;

public class ElectricityBill {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of units consumed: ");
        int units = sc.nextInt();
        double bill;

        if (units <= 100) {
            bill = units * 1.50;
        } else if (units <= 300) {
            bill = 100 * 1.50 + (units - 100) * 2.50;
        } else {
            bill = 100 * 1.50 + 200 * 2.50 + (units - 300) * 4.00;
        }

        System.out.println("Electricity Bill: " + bill);
    }
}

Output

Enter number of units consumed: 350  
Electricity Bill: 875.0
