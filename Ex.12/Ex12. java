import java.util.*;

class Student {
    private int rollNo;
    private String name;
    private double attendance;

    Student(int rollNo, String name, double attendance) {
        this.rollNo = rollNo;
        this.name = name;
        this.attendance = attendance;
    }

    public int getRollNo() {
        return rollNo;
    }

    public String getName() {
        return name;
    }

    public double getAttendance() {
        return attendance;
    }

    public void setAttendance(double attendance) {
        this.attendance = attendance;
    }

    public void display() {
        System.out.println("Roll Number : " + rollNo);
        System.out.println("Student Name : " + name);
        System.out.println("Attendance : " + attendance + "%");
    }
}

public class StudentAttendanceLookup {
    public static void main(String[] args) {

        HashMap<Integer, Student> students = new HashMap<>();

        students.put(101, new Student(101, "Arun", 85.5));
        students.put(102, new Student(102, "Priya", 78.0));
        students.put(103, new Student(103, "Kavin", 92.5));

        int searchRoll = 102;

        System.out.println("Student Details");
        System.out.println("----------------");

        if (students.containsKey(searchRoll)) {
            Student s = students.get(searchRoll);
            s.display();

            s.setAttendance(88.0);

            System.out.println("\nAfter Attendance Update");
            System.out.println("-----------------------");
            s.display();
        } else {
            System.out.println("Student not found");
        }
    }
}