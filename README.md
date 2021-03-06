// ElectricCar937
//CodeHS 9.3.7

public class ElectricCar extends Car {

    // Complete the constructor
    public ElectricCar(String model, String mpg)
    {
      super(model, mpg);
    }

    // Override the getMPG here.
    // It should return: "Electric cars do not calculate MPG.

    public String getMPG()
    {
        return "Electric cars do not calculate MPG.";
    }
    // Override the toString() here.
    // (model) is an  electric car.
    @Override
    public String toString()
    {
        return getModel() + " is an electric car.";
    }
    
    
}


public class Car {

    //This code is complete
    private String model;
    private String mpg;

    public Car(String model, String mpg){
        this.model = model;
        this.mpg = mpg;
    }

    public String getModel(){
        return model;
    }

    public String getMPG(){
        return mpg;
    }

    public String toString(){
        return model + " gets " + mpg + " mpg.";
    }
}


public class CarTester
{
    public static void main(String[] args)
    {
        // Create a Car object
        Car a = new Car("Model S", "23");
        // Print out the model
        System.out.println(a.getModel());
        // Print out the MPG
        System.out.println(a.getMPG());
        // Print the object
        System.out.println(a.toString());
        // Create an ElectricCar object
        ElectricCar b = new ElectricCar("Model B", "76");
        // Print out the model
        System.out.println(b.getModel());
        // Print out the MPG
        System.out.println(b.getMPG());
        // Print the object
        System.out.println(b.toString());
    }
}
