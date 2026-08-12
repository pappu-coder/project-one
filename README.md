# project-one
import java.util.Scanner;
public class Equations {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // (a) Area of cylinder = πr² + 2πrh
        System.out.print("Enter radius (r): ");
        double r = sc.nextDouble();
        System.out.print("Enter height (h): ");
        double h = sc.nextDouble();
        double Area = Math.PI * r * r + 2 * Math.PI * r * h;
        System.out.println("Area of cylinder = " + Area);
        System.out.println();

        // (b) Torque = (2 * m1 * m2) / (m1 + m2) * g
        System.out.print("Enter m1: ");
        double m1 = sc.nextDouble();
        System.out.print("Enter m2: ");
        double m2 = sc.nextDouble();
        System.out.print("Enter g: ");
        double g = sc.nextDouble();
        double Torque = (2 * m1 * m2*g) / (m1 + m2);
        System.out.println("Torque = " + Torque);
        System.out.println();

        // (c) Side = √(a² + b² − 2ab cos(x))
        System.out.print("Enter a: ");
        double a = sc.nextDouble();
        System.out.print("Enter b: ");
        double b = sc.nextDouble();
        System.out.print("Enter x (in radians): ");
        double x = sc.nextDouble();
        double Side = Math.sqrt(a * a + b * b - 2 * a * b * Math.cos(x));
        System.out.println("Side = " + Side);
        System.out.println();

        // (d) Energy = mass * (acceleration * height + velocity² / 2)
        System.out.print("Enter mass: ");
        double mass = sc.nextDouble();
        System.out.print("Enter acceleration: ");
        double acceleration = sc.nextDouble();
        System.out.print("Enter height: ");
        double height = sc.nextDouble();
        System.out.print("Enter velocity: ");
        double velocity = sc.nextDouble();
        double Energy = mass * (acceleration * height + velocity * velocity / 2);
        System.out.println("Energy = " + Energy);

        sc.close();
    }
}
