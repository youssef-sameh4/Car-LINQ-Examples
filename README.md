# Car-LINQ-Examples



---

##  Car Class

public class Car
{
    public Car(int id, string make, string color, int maxSpeed)
    {
        Id = id;
        Make = make;
        Color = color;
        MaxSpeed = maxSpeed;
    }

    public int Id { get; set; }
    public string Make { get; set; }
    public string Color { get; set; }
    public int MaxSpeed { get; set; }
}


# Repository
public class CarRepository
{

    public static IEnumerable<Car> GetCars()
    {
        return new List<Car>
    {
        new Car(1, "BMW", "Red", 240),
        new Car(2, "Audi", "Black", 230),
        new Car(3, "Mercedes", "White", 250),
        new Car(4, "Toyota", "Blue", 180),
        new Car(5, "Honda", "Gray", 170),
        new Car(6, "Ford", "Red", 200),
        new Car(7, "Chevrolet", "Black", 210),
        new Car(8, "Nissan", "White", 190),
        new Car(9, "Hyundai", "Blue", 175),
        new Car(10, "Kia", "Gray", 165),
        new Car(11, "Tesla", "White", 260),
        new Car(12, "Volkswagen", "Black", 185),
        new Car(13, "Peugeot", "Blue", 170),
        new Car(14, "Renault", "Red", 160),
        new Car(15, "Mazda", "Gray", 180),
        new Car(16, "Subaru", "White", 200),
        new Car(17, "Jeep", "Black", 220),
        new Car(18, "Volvo", "Blue", 210),
        new Car(19, "Lexus", "Gray", 240),
        new Car(20, "Porsche", "Red", 300),
        new Car(21, "BMW", "Blue", 245),
        new Car(22, "Audi", "Red", 235),
        new Car(23, "Mercedes", "Black", 255),
        new Car(24, "Toyota", "White", 185),
        new Car(25, "Honda", "Red", 175),
        new Car(26, "Ford", "Blue", 205),
        new Car(27, "Chevrolet", "Gray", 215),
        new Car(28, "Nissan", "Black", 195),
        new Car(29, "Hyundai", "Red", 180),
        new Car(30, "Kia", "White", 170)

    };
    }
    public static void PrintCars(IEnumerable<Car> cars)
    {
        foreach (var car in cars)
        {
            Console.WriteLine($"ID: {car.Id} |  Make: {car.Make} |   Color: {car.Color} |  MaxSpeed: {car.MaxSpeed} km/h");
        }
    }
}
