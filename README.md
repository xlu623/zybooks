import java.util.Random;
import java.util.Scanner;

public class RandomGenerator {

	public static void main(String[] args) {

      
      Random randGen = new Random(Config.SEED);
      Scanner scnr = new Scanner(System.in);
      
      System.out.println("Random Number Calculator");
      
      int minInt = 0 ;
      System.out.print("Enter minimum integer: ");
      minInt = scnr.nextInt();
      
      
      int maxInt=0;
      System.out.print("Enter maximum integer: ");
      maxInt = scnr.nextInt();
      
      
      System.out.println("Three integers are: ");
      System.out.println(randGen.nextInt(maxInt-minInt+1)+minInt);
      System.out.println(randGen.nextInt(maxInt-minInt+1)+minInt);
      System.out.println(randGen.nextInt(maxInt-minInt+1)+minInt);
      
	}
}
