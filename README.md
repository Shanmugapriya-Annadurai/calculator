import java.util.*;
class Calculator {
    public double add(double a, double b) {
        return a+b;
    }
    public double subtract(double a, double b) {
        return a-b;
    }
    public double multiply(double a, double b) {
        return a*b;
    }
    public double divide(double a, double b) {
        if (b==0) {
            System.out.println("Error: Division by zero is undefined.");
            return 0;
        }
        return a/b;
    }
}
public class calc{
    public static void main(String[] args) {
        Scanner scan=new Scanner(System.in);
        Calculator calc=new Calculator();

        double num1=scan.nextDouble();
        double num2=scan.nextDouble();

        System.out.println("Addition: "+calc.add(num1, num2));
        System.out.println("Subtraction: "+calc.subtract(num1, num2));
        System.out.println("Multiplication: "+calc.multiply(num1, num2));
        System.out.println("Division: "+calc.divide(num1, num2));
    }
}
