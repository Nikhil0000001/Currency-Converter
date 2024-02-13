# Currency-Converter
import java.util.Scanner;

public class CurrencyConverter {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Enter the amount to convert:");
        double amount = scanner.nextDouble();

        System.out.println("Enter the exchange rate from USD to your currency:");
        double exchangeRate = scanner.nextDouble();

        double convertedAmount = convertCurrency(amount, exchangeRate);

        System.out.println(amount + " USD is equal to " + convertedAmount + " in your currency.");
    }

    private static double convertCurrency(double amount, double exchangeRate) {
        return amount * exchangeRate;
    }
}
