```jsx
ЗАДАЧА №1

import java.util.Scanner;


class Homework2 {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.println("Ведите число: ");

        int number = scan.nextInt();
        if (number % 2 == 0) {
            System.out.println("Это чилсо четное");
        } else {
            System.out.println("Это число нечетное");
        }
    }


}


ЗАДАЧА №2

class Homework2 {
    public static void main(String[] args) {
        for (int i = 3; i == 3; i++) {
            for (int j = 1; j <= 10; j++) {
                System.out.println(i + "x" + j + "=" + i * j );
            }

        }

     }
     
     
     ЗАДАЧА№3
     import java.util.Scanner;

public class Homework2 {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);

        System.out.println("Ведите год в формате \"yyyy\"");
        int year = scan.nextInt();
        if ((year % 400 == 0) || (year % 4 == 0) && (year != 0)) {
            System.out.println(year + " Этот год високосный, в нем 366 дней");
        } else {
            System.out.println(year + " Этот год  НЕ високосный, в нем 365 дней");
        }


    }
}
}
