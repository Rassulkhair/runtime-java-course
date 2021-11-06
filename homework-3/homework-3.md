```jsx
ЗАДАЧА №1

public class Car {         //Нужно создать класс Car, где я описываю объект и его поведение 
    String brand;
    String model;
    int speed;            //Здесь я  описываю состояние  объкта, т.е. то что в него будет вложенно. В данном случае я описываю бренд, модель и скорость 

    public void start() {
        System.out.println("Бренд: " + brand);
        System.out.println("Модель: " + model);
        System.out.println("Скорость: " + speed);

    }                   // В этом блоке я создаю метод, иными словами поведение объкта, что он должен будет делать при вызове 

    public void stop() {
        System.out.println("Бренд: " + brand);
        System.out.println("Модель: " + model);
        System.out.println("Скорость: " + speed);

    }                 // Этот блок кода, также является методом, с таким же смыслом, что и выше. Это нужно для второго объекта


}

public class Test {             // Это следующий класс, который я исппользую с целью создания и описания объктов. 
    public static void main(String[] args) {   //Это блок main, отправная точка выполнение задач 
        
        Car car1 = new Car();
        Car car2 = new Car();  // Здесь я создаю два объкта, над которыми я буду выполнять последующие действия
        
        car1.brand = "Toyota";
        car1.model = "Camry";
        car1.speed = 80;    // В  объекте Car1, я задаю описание объкта, его сущности. Использую оператор <.>, своего рода это вызов того или иного параметра и занимаюсь 
                            // присваиванием обозначений 
        
        car2.brand = "Mustang";
        car2.model = "idkw";
        car2.speed = 65;  // Такая же операция, что и проводилась в Car1, только уже для второго объекта Car2
        
        System.out.println("Добро пожаловать в католог машин!");
        System.out.println();
        
        System.out.println("Информация об первой машине: ");
        System.out.println();
        car1.start();   // Здесь я уже вызываю метод start, который был создан в классе Car. В классе Car указанна задача для этого объкта (выводить данные)
        System.out.println();
        
        System.out.println("Информация об второй машине: ");
        System.out.println();
         car2.stop();  // Здесь я уже вызываю метод stop, который был создан в классе Car. В классе Car указанна задача для этого объкта (выводить данные)

    }
}



ЗАДАЧА №2

public class Human {  
    public void printName(String surname, String name) { // Здесь создается метод с двумя параметрами, которые будут описанны в другом классе 

        System.out.println("Ваша фамилия: " + surname + " " + "Ваше имя: " + name);

    } // В этом блоке кода указаны задачи для JVM

}

public class Test {
    public static void main(String[] args) {
        Human person = new Human(); //Создали объект 
        person.printName("Shokanov", "Rassulkhair"); // Эта строка кода служит для вызова метода, что должен делать объет и описание параметров объекта (Это аргументы) 
                                                     // Важно помнить порядок присаивания, то есть, аргумент написанный первый идет к первому параметру, соответсвенно второй к 
                                                     // второму. Также стоит быть внимательным к типу данных 

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
        int a = 2;
        int b = 5;
        int c = 3;
        solution.printSum(var1, var2, var3);


    }
}  //Логика решения задачи такая же, как и в прошлых двух


ЗАДАЧА №4

public class Age {
    public void printAge(int age, int year) {
        int x = 2;
        int y = 2019;
        int z = x + age;
        int v = year - y;
        System.out.println(z + " " + v);  // Здесь другой подход отличающийся от других задач, где я использую такое понятие, как локальные переменные 
                                          // Локальные переменные это те переменные, созданные в классе, которые служат для создания описания и задач, которые должна выполнять 
                                          // JVM для будущего объкта 


    }

}

public class Test {
    public static void main(String[] args) {
        Age variable = new Age();
        variable.printAge(20, 2018);


    }
}


ЗАДАЧА №5

public class Return {  // Создаю класс, в котором будут созданны методы, для описания  двух будущих объктов. Здесь я столкнусь с таким оператором, как return
    int printNumber() {  // Я создал метод printNumber(), который будет использоваться для первого объкта
        return 24 + 1;  // Оператор return служит для того, чтобы возвращать значения и вкладывать его смысл в объект\метод. 

    }

    int printNumber2() {
        return 22 + 2;  // Тоже самое, что и выше 
    }
}


public class Test {

    public static void main(String[] args) {
        Return returnNumber = new Return();  // Создаю объкт для первого значения(25)
        int number = returnNumber.printNumber(); //Создаю параметр number с типом int, и приравниваю его к объкту, в котором вызываю метод. То есть значение, которое было в 
                                                 // первом методе (операция 24+1) ВОЗВРАЩАЕТСЯ/ПРИСВАЕВАЕТСЯ к параметру number. 
        System.out.println(number); // Вывожу на консоль параметр number 


        Return returnNumber2 = new Return();
        int number2 = returnNumber2.printNumber2();
        System.out.println(number2); //Тоже самое, что и выше 
    }

}






ЗАДАЧА №6 
public class Test {

        public static void main (String[]args){
            System.out.println(getHelloMessage());
        }

        public static String getHelloMessage () {
            return "Hello World";
        }

    }   //логика в том, что значение return ("Hello World"), который следует за новым методом, переходит в getHelloMessage и выводит его на консоль
