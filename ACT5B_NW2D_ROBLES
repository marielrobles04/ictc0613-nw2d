package act5;
import java.util.*;

public class ACT5B_NW2D_ROBLES {
    public String first;
    public String last;
    public String middle;
    public String gender;
    public int aCode;
    public int age;
    public long telnum;
    public ACT5B_NW2D_ROBLES next;
    public static ACT5B_NW2D_ROBLES firstNode;
    public static ACT5B_NW2D_ROBLES lastNode=null;
    
    public ACT5B_NW2D_ROBLES(String fn, String ln, String mn, String g, int a, int ac, long t, ACT5B_NW2D_ROBLES n){
        first = fn;
        last = ln;
        middle = mn;
        gender = g;
        age = a;
        aCode = ac;
        telnum = t;
        next=n;
    }
    public static void main(String[] args) {
       Scanner s = new Scanner (System.in);
      int memberNum, aCode, age ;
      String first, last, middle, gender;
      long telnum;
     
       System.out.print("How many member's information will be entered? ");
       memberNum = s.nextInt();
      
       for (int i = 0; i<memberNum; i++){
           System.out.println("\nKindly give the information of member # " + (i+1));
           first=s.nextLine();
           System.out.print("Input First Name: ");
           first=s.nextLine();
           
           System.out.print("Input Middle Name: ");
           middle=s.nextLine();
           
           System.out.print("Input Last Name: ");
           last=s.nextLine();
           
           System.out.print("Input Area Code: ");
           aCode=s.nextInt();
           
           System.out.print("Input Telephone Number: ");
           telnum=s.nextLong();
           
           gender=s.nextLine();
           System.out.print("Input Gender: ");
           gender=s.nextLine();
           
           System.out.print("Input Age: ");
           age=s.nextInt(); 
           
           ACT5B_NW2D_ROBLES list = new ACT5B_NW2D_ROBLES (first, last, middle, gender, age, aCode, telnum, null);
           if (lastNode!=null){
                lastNode.next=list;
                lastNode=list;
            }
            else
            {
                firstNode=list;
                lastNode=list;
            }    
    }
       
         ACT5B_NW2D_ROBLES list= firstNode;
         while (list!=null)
         {
             System.out.print("\nWelcome to the club " + list.first + " "+ list.middle + " " +list.last + "!" + "\n");
             System.out.print("Your code and telephone number is " + "("+list.aCode+") " + list.telnum + "\n");
             System.out.print("You are a "+ list.gender + " and your age is " + list.age + "." + "\n");
             list=list.next;
         }     
}
}
