






import java.util.Scanner;
public class RowdyHackers {
 public static void main(String[] args) {
     Scanner scnr = new Scanner (System.in);
     System.out.println("Rowdy Hacks: Hackathon");
     System.out.println("Grade Calculator");
     System.out.println();
     System.out.print("How many homework assignments did you have? "); 
     int userNum=scnr.nextInt();
     System.out.print("What grade did you get? ");
     int ptsEarn=scnr.nextInt();
     System.out.println();
     System.out.println();

     int totalHw = (userNum * ptsEarn);
     int possiblePts=5;
     

     System.out.print("Homework" + "\t" + "\t" + "Points Earned" + "\t" + "Possible Points");
     
     for (int i=0; i<=userNum; i++) {                            // outer loop for number of hw items
       System.out.print(i + "\t" + "\t");
       
       if (ptsEarn >0 && ptsEarn <=5) {                          // inner loop for points earned
         System.out.print (ptsEarn + "\t" + "\t");
         
         for (possiblePts=5; possiblePts<=5; possiblePts++) {    // inner loop for possible points
         System.out.print(possiblePts);
        
      
         System.out.println();
         }
       }
     }
     
     System.out.println("Total Homework grade: " + totalHw);
     System.out.println("Total possible points: " + possiblePts);
     System.out.println();    
     System.out.println();

     
     System.out.print("How many quizzes did you have? "); 
     int quizNum=scnr.nextInt();
     System.out.print("What grade did you get? ");
     int quizGrade=scnr.nextInt();
     System.out.println();

     int totalQuiz;
     
     totalQuiz = (quizNum * quizGrade);
      
      System.out.print("Quiz" + "\t" + "\t" + "Points Earned" + "\t" + "Possible Points");
      
     for (int j=0; j<=quizNum; j++) {                            // outer loop for number of hw items
       System.out.print(j + "\t" + "\t");
       
       if (quizGrade >0 && quizGrade <=5) {                                     // inner loop for points earned
         System.out.print (quizGrade + "\t" + "\t");
         
         for (int possiblePts1=5; possiblePts1<=5; possiblePts1++) {    // inner loop for possible points
         System.out.print(possiblePts1);
        
      
         System.out.println();
         }
       }
     }
     
     System.out.println("Total quiz grade: " + totalQuiz);
     
     System.out.println();    
     System.out.println();

     
     System.out.print("How many exams did you have? "); 
     int examNum=scnr.nextInt();
     System.out.print("What grade did you get? ");
     int examGrade=scnr.nextInt();
     System.out.println();
     
      int totalExam = (examNum * examGrade);
      int finalGrade = totalHw + totalQuiz + totalExam;
      
      
      System.out.print("Exam" + "\t" + "\t" + "Points Earned" + "\t" + "Possible Points");
      
     for (int k=0; k<=examNum; k++) {                            // outer loop for number of hw items
       System.out.print(k + "\t" + "\t");
       
       if (examGrade >0 && examGrade <=100) {                                     // inner loop for points earned
         System.out.print (examGrade + "\t" + "\t");
         
         for (int possiblePts2=100; possiblePts2<=100; possiblePts2++) {    // inner loop for possible points
         System.out.print(possiblePts2);
         
         System.out.println();
         
         
         }  
     }
     }
        
     
     System.out.println("Total exam grade: " + totalExam);
     System.out.println("Total grade: " + finalGrade);

 }
}
         
