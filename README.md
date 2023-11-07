# Ex-10
```
class Member {
    String name;
    int age;
    String phoneNumber;
    String address;
    double salary;
    Member(String name, int age, String phoneNumber, String address, double salary) {
        this.name = name;
        this.age = age;
        this.phoneNumber = phoneNumber;
        this.address = address;
        this.salary = salary;
    }
    void printSalary() {
        System.out.println("Salary: " + salary);
    }
}
class Employee extends Member {

    String specialization;
    Employee(String name, int age, String phoneNumber, String address, double salary, String specialization) {
        super(name, age, phoneNumber, address, salary);
        this.specialization = specialization;
    }
}

class Manager extends Member {

    String department;

    Manager(String name, int age, String phoneNumber, String address, double salary, String department) {
        super(name, age, phoneNumber, address, salary);
        this.department = department;
    }
}

public class Main {
    public static void main(String[] args) {

        Employee employee = new Employee("John Doe", 30, "1234567890", "123 Main St", 50000.0, "Software Developer");
        Manager manager = new Manager("Jane Smith", 35, "9876543210", "456 Broad St", 80000.0, "HR");

        System.out.println("Employee Details:");
        System.out.println("Name: " + employee.name);
        System.out.println("Age: " + employee.age);
        System.out.println("Phone Number: " + employee.phoneNumber);
        System.out.println("Address: " + employee.address);
        employee.printSalary();
        System.out.println("Specialization: " + employee.specialization);
        System.out.println();
        System.out.println("Manager Details:");
        System.out.println("Name: " + manager.name);
        System.out.println("Age: " + manager.age);
        System.out.println("Phone Number: " + manager.phoneNumber);
        System.out.println("Address: " + manager.address);
        manager.printSalary();
        System.out.println("Department: " + manager.department);
    }
}

```
#Output
![Screenshot (74)](https://github.com/21002624/Ex-10/assets/113762183/eddcc743-280a-4de6-86c2-8e2552f2ef92)
