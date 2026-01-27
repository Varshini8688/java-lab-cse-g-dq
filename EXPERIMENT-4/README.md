## Experiment-4a
## Title:Implementing single inheritance
## Source Code:
``` java
class Person{
    String name;
    int age;
    Person(String name,int age){
      this.name= name;
      this.age= age;
    }
    void displayPersonDetails(){
         System.out.println("Name: " + name);
         System.out.println("Age: " + age);
   }
 }
class Employee extends Person{
     double annualSalary;
     int YearofJoining;
     String NationalInsuranceNumber;
     Employee(String name,int age,double annualSalary,int YearofJoining,String NationalInsuranceNumber){
     super(name, age);
     this.annualSalary = annualSalary;
     this.YearofJoining = YearofJoining;
     this.NationalInsuranceNumber = NationalInsuranceNumber;
     }
     void displayEmployeeDetails() {
          displayPersonDetails();
          System.out.println("Annual Salary: " + annualSalary);
          System.out.println("national Insurance Number: " + NationalInsuranceNumber);
       }
   }
class Main{
    public static void main( String[] args){
          Employee emp = new Employee("varshini",20,500000.0,2025,"NI12345");
          emp.displayEmployeeDetails();
    }
 }
```
## Output:
![EXp-4a Output](person.png)
   
