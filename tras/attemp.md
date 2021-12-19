```jsx
public class Cat {
    String name;
    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;

    }
    public void run() {
        System.out.println("Бег");
    }


}


public class Lion extends Cat {
    String name= "Лев";

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;

    }

    @Override

    public void run() {
        System.out.println("Лев бежит со скоростью 80 км/ч");
    }
}



public class Tiger extends Cat {
    String name= "Тигр";
    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;

    }
    @Override
    public void run() {
        System.out.println("Тигр бежит со скоростью 60 км/ч");
    }
}


public class Cheetah extends Cat {
    String name="Гепард";
    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;

    }
    @Override
    public void run() {
        System.out.println("Гепард бежит со скоростью 120 км/ч");
    }
}



public class Doctor {
    public void healcat(Cat cat) {
        System.out.println(cat.getName() + " " + "здоров");
        cat.run();
    }

}



public class Test {
    public static void main(String[] args) {
        Lion simba = new Lion();
        Tiger tigra = new Tiger();
        Cheetah cheek = new Cheetah();
        Doctor doctorAibolit = new Doctor();

        doctorAibolit.healcat(simba);
        doctorAibolit.healcat(tigra);
        doctorAibolit.healcat(cheek);


    }
}
