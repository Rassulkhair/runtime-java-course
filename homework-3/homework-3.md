```jsx
ЗАДАЧА №1

public class Car {
    String brand;
    String model;
    int speed;

    public void start() {
        System.out.println("Бренд: " + brand);
        System.out.println("Модель: " + model);
        System.out.println("Скорость: " + speed);

    }

    public void stop() {
        System.out.println("Бренд: " + brand);
        System.out.println("Модель: " + model);
        System.out.println("Скорость: " + speed);

    }


}

public class Test {
    public static void main(String[] args) {
        Car car1 = new Car();
        Car car2 = new Car();
        car1.brand = "Toyota";
        car1.model = "Camry";
        car1.speed = 80;
        car2.brand = "Mustang";
        car2.model = "idkw";
        car2.speed = 65;
        System.out.println("Добро пожаловать в католог машин!");
        System.out.println();
        System.out.println("Информация об первой машине: ");
        System.out.println();
        car1.start();
        System.out.println();
        System.out.println("Информация об второй машине: ");
        System.out.println();
        car2.stop();

    }
}



ЗАДАЧА №2

public class Human {
    public void printName(String surname, String name) {

        System.out.println("Ваша фамилия: " + surname + " " + "Ваше имя: " + name);

    }

}

public class Test {
    public static void main(String[] args) {
        Human person = new Human();
        person.printName("Shokanov", "Rassulkhair");


    }
}

ЗАДАЧА №3
public class Calc {
    public void printSum(int a, int b, int c) {
        int z = a + b + c;
        System.out.println("Сумма трех чисел равна: " + z);


    }

}

public class Test {
    public static void main(String[] args) {
        Calc solution = new Calc();
        int var1 = 2;
        int var2 = 5;
        int var3 = 3;
        solution.printSum(var1, var2, var3);


    }
}


ЗАДАЧА №4

public class Age {
    public void printAge(int age, int year) {
        int x = 2;
        int y = 2019;
        int z = x + age;
        int v = year - y;
        System.out.println(z + " " + v);


    }

}

public class Test {
    public static void main(String[] args) {
        Age variable = new Age();
        variable.printAge(20, 2018);


    }
}


ЗАДАЧА №5

