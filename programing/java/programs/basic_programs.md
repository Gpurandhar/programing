# Java Solutions

### 1) Calculate Simple Interest
**Question:** Write a Java program to calculate the simple interest given the principal, rate of interest, and time period.
```java
import java.util.Scanner;
public class SimpleInterest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter Principal: ");
        double principal = sc.nextDouble();
        System.out.print("Enter Rate: ");
        double rate = sc.nextDouble();
        System.out.print("Enter Time: ");
        double time = sc.nextDouble();
        double interest = (principal * rate * time) / 100;
        System.out.println("Simple Interest: " + interest);
    }
}
```

### 2) Convert Fahrenheit to Celsius
**Question:** Write a Java program to convert temperature from Fahrenheit to Celsius.
```java
import java.util.Scanner;
public class TemperatureConversion {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter Fahrenheit: ");
        double fahrenheit = sc.nextDouble();
        double celsius = (fahrenheit - 32) * 5/9;
        System.out.println("Celsius: " + celsius);
    }
}
```

### 3) Calculate Area and Circumference of Circle
**Question:** Write a Java program to calculate the area and circumference of a circle given its radius.
```java
import java.util.Scanner;
public class Circle {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter Radius: ");
        double radius = sc.nextDouble();
        double area = Math.PI * radius * radius;
        double circumference = 2 * Math.PI * radius;
        System.out.println("Area: " + area);
        System.out.println("Circumference: " + circumference);
    }
}
```

### 4) Arithmetic Operations
**Question:** Write a Java program to perform all basic arithmetic operations (addition, subtraction, multiplication, division, and modulus) on two numbers.
```java
import java.util.Scanner;
public class ArithmeticOperations {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter two numbers: ");
        double a = sc.nextDouble();
        double b = sc.nextDouble();
        System.out.println("Addition: " + (a + b));
        System.out.println("Subtraction: " + (a - b));
        System.out.println("Multiplication: " + (a * b));
        System.out.println("Division: " + (a / b));
        System.out.println("Modulus: " + (a % b));
    }
}
```

### 5) Calculate BMI
**Question:** Write a Java program to calculate the Body Mass Index (BMI) given weight (kg) and height (m).
```java
import java.util.Scanner;
public class BMI {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter weight (kg): ");
        double weight = sc.nextDouble();
        System.out.print("Enter height (m): ");
        double height = sc.nextDouble();
        double bmi = weight / (height * height);
        System.out.println("BMI: " + bmi);
    }
}
```

### 6) Area and Perimeter of Rectangle
**Question:** Write a Java program to calculate the area and perimeter of a rectangle given its length and breadth.
```java
import java.util.Scanner;
public class Rectangle {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter Length: ");
        double length = sc.nextDouble();
        System.out.print("Enter Breadth: ");
        double breadth = sc.nextDouble();
        System.out.println("Area: " + (length * breadth));
        System.out.println("Perimeter: " + (2 * (length + breadth)));
    }
}
```

### 7) Special Digits
**Question:** Write a Java program to check if a two-digit number is a special number (e.g., 89 → 8+9+8*9 = 89).
```java
import java.util.Scanner;
public class SpecialDigit {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter two-digit number: ");
        int num = sc.nextInt();
        int d1 = num / 10;
        int d2 = num % 10;
        if ((d1 + d2 + d1 * d2) == num) {
            System.out.println("Special Number");
        } else {
            System.out.println("Not a Special Number");
        }
    }
}
```

### 8) Even or Odd
**Question:** Write a Java program to check whether a number is even or odd.
```java
import java.util.Scanner;
public class EvenOdd {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int num = sc.nextInt();
        if (num % 2 == 0)
            System.out.println("Even");
        else
            System.out.println("Odd");
    }
}
```

### 9) Voting Eligibility
**Question:** Write a Java program to check if a person is eligible to vote (age should be 18 or above).
```java
import java.util.Scanner;
public class Voting {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter age: ");
        int age = sc.nextInt();
        if (age >= 18)
            System.out.println("Eligible to vote");
        else
            System.out.println("Not eligible to vote");
    }
}
```

### 10) Product Price Calculation
**Question:** Write a Java program to read the price of a product, calculate the total amount, and determine how much change needs to be returned to the customer.
```java
import java.util.Scanner;
public class ProductPrice {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter total amount: ");
        double totalAmount = sc.nextDouble();
        System.out.print("Enter amount given by customer: ");
        double givenAmount = sc.nextDouble();
        double change = givenAmount - totalAmount;
        System.out.println("Change to return: " + change);
    }
}
```
