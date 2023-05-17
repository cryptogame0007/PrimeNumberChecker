# PrimeNumberChecker
PrimeNumberChecker
import java.util.Scanner;

public class PrimeNumberChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Введите число: ");
        int number = scanner.nextInt();

        boolean isPrime = checkPrime(number);
        if (isPrime) {
            System.out.println("Число является простым!");
        } else {
            System.out.println("Число не является простым.");
        }
    }

    public static boolean checkPrime(int number) {
        if (number <= 1) {
            return false;
        }
        for (int i = 2; i <= Math.sqrt(number); i++) {
            if
