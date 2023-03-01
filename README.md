# Code-for-Class-file-Dog.java-

public class Dog extends Animal implements IPettable {

    protected static final int dogToHumanYearMultiplier = 7;

    public int getAgeInHumanYears() {
        return  age * dogToHumanYearMultiplier;
    }



    public Dog(String picture, String name, int age) {
       super(picture, name, age);
    }

    @Override
    public void madeSound() {
        System.out.println(this.name + " woofed!");
    }

    @Override
    public void pet() {
        System.out.println(this.name + " is such a happy pet");


  }
}
