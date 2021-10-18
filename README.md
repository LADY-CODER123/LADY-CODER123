import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner input = new Scanner (System.in);

        boolean isvaccinationdone = true;
        while(isvaccinationdone){
            System.out.println("Have you done your vaccination? Yes or no ");
            String userfirstinput = input.next("no");
            System.out.println("Its mandatory to take two doses of vaccine");

            String userinput = input.next("yes");
            System.out.println("Please mention the number of doses that you have taken");
            int numberofvaccination = input.nextInt();


            if (userinput.equals("yes")){
                isvaccinationdone = false;
            }


            if(numberofvaccination==2){
                System.out.println("Well done Stay Home Stay Safe!");
            }

            if(numberofvaccination<2){
                System.out.println("Please take your second dose vaccination immediately");
            }








        }



    }
}
