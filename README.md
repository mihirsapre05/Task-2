import java.util.Scanner;

public class Task_2 {
    public static void main(String[] args) {
        ///student Grade Calculator

        Scanner sc = new Scanner(System.in);
        System.out.println("Student Grade Calculator");
        System.out.println("Enter no of subjects");
        int ns= sc.nextInt();
        int total =0;
        for(int i=0;i<ns;i++){
            System.out.println("Enter marks obtained in "+i+1+":");
            int marks= sc.nextInt();
            total+=marks;
        }
        double averP=(double)total/ns;
        char grade;
        if (averP>=90){
            grade='O';
        }
        else if (averP>=80) {
            grade='A';
        }
        else if (averP>=70) {
            grade='B';

        }
        else if (averP>=60) {
            grade='C';

        }
        else if (averP>=50) {
            grade='D';

        }
        else if (averP>=40) {
            grade='E';

        }
        else {
            grade='F';
        }
        System.out.println("Total Marlks Scored is"+total);
        System.out.println("Average Percentage Gained is "+averP+"%");
        System.out.println("Grade :"+grade);


    }
}
