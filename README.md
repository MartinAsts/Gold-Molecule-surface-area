# Gold-Molecule-surface-area
import java.util.Scanner;
import java.util.Random;

public class TableAreaCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Random random = new Random();
        // 13.074
        // 52.296
        // System.out.println("Enter the length of the base 1 (in nanometers): ");
        double length = 4.08 + random.nextDouble(4.08);

        // System.out.println("Enter the width of the base2 (in nanometers): ");
        double width = 4.08 + random.nextDouble(4.08);

        // System.out.println("Enter the height (in nanometers): ");
        double height = 4.08 + random.nextDouble(4.08);

        double area = calculateArea(length, width, height);
        System.out.println("Free surface area: " + area + " %.");
    }

    public static double calculateArea(double length, double width, double height) {
        return ((((length + width) / 2 * height) - 13.074) / (((length + width) / 2 *
                height) + 39.222)) * 100;

    }

}
