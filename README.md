import java.util.Scanner;

public class App {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);
        int students;

        System.out.print("Enter number of students: ");
        students = scanner.nextInt();
        scanner.nextLine();

        for (int i = 1; i <= students; i++) {

            studentGrade(scanner);

        }
        

        scanner.close();
    }
    // student grade func
    static void studentGrade(Scanner scanner) {
        
        
        System.out.print("Enter student's name: ");
        String name = scanner.nextLine();
        
        System.out.print("Enter grade for subject 1: ");
        int subject1 = scanner.nextInt();
        
        System.out.print("Enter grade for subject 2: ");
        int subject2 = scanner.nextInt();

        System.out.print("Enter grade for subject 3: ");
        int subject3 = scanner.nextInt();
        scanner.nextLine();
        // calculate average
        double avr = (subject1 + subject2 + subject3) / 3.0;
        System.out.printf("%s's average grade: %.2f%n", name, avr);
    }
    

}
