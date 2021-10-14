# Total-Salary
import java.util.Scanner;
public class Main {	
	public static void main(String[] args) {
        int basic ,allow;
        double  totalSalary ,hra ,da ,pf;
        Scanner s = new Scanner(System.in);
        // System.out.println("Enter basic salary ");
        basic = s.nextInt();
         // System.out.println("Enter grade ");
        String str =s.next();
        char grade = str.charAt(0);
        
        hra = 0.2*basic;
        da = 0.5*basic;
        pf = 0.11*basic;

       if(grade=='A') {
        allow=1700;} 
        else if(grade=='B'){ 
           allow=1500;}
        else{
         allow=1300 ;
          }
        totalSalary = basic + hra + da + allow - pf;
        System.out.println(Math.round(totalSalary));
	}
}
