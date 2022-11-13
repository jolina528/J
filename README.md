package hardcoding;
import java.util.Scanner;

public class Main{

  public static void main(String[]args) {
  
  Scanner console = new Scanner(System.in);
  
  
  String orderCart = "Your orders are the following: \n";
  int respondToOrder, orderCategory;
  float totalPayment = 0, customerCash;
  
  System.out.println("==========WELCOME TO MANG KULAFS TAGAYAN! ========");
  System.out.println("| DO YOU WANT TO ORDER? [1-YES, 2-NO]            |");
  System.out.println("| Enter the number for your choice below         |");
  System.out.println("==================================================");
  System.out.print  ("Choice:");
  respondToOrder = console.nextInt(); 
  
  do {

  if (respondToOrder == 1) {
  
	  System.out.println("==========WELCOME TO MANG KULAFS TAGAYAN! ========");
	  System.out.println("|WHAT TO ORDER? [1-FOOD, 2 - BEVERAGES , 3-SNACKS|");
	  System.out.println("| Enter the number for your choice below         |");
	  System.out.println("==================================================");
	  System.out.print  ("Choice:");
	  orderCategory = console.nextInt();
	  
	  if(orderCategory == 1) {
	    System.out.println("==========WELCOME TO MANG KULAFS TAGAYAN! ========");
	    System.out.println("|***************ORDER FOOD***********************|");
	    System.out.println("| [1] Unli-Chicken Wings + Unli-Rice : P250.00   |");
	    System.out.println("| [2] Unli-Pork Fat + Sisig          : P180.00   |");
	    System.out.println("| [3] Bangus Sisig + Unli-Rice       : P180.00   |");
	    System.out.println("| Enter the number for your choice below         |");
	    System.out.println("==================================================");
	    System.out.print  ("Choice:");
	    float unliChicken = 250 , unliPork = 180, bangusSisig = 180;
	    int orderChoice = console.nextInt();
	    
	      switch (orderChoice) {
		case 1: 
		  System.out.println("Unli-Chicken Wings + Unli-Rice: P250.00 added to cart");
		  totalPayment+=unliChicken;
		  String order1 = "Unli-Chicken Wings + Unli-Rice: P250.00 \n";
		  orderCart+=order1;
		  
		break;
		
		case 2: 
		  System.out.println("Unli-Pork Fat + Sisig P 180   : P180.00  added to cart");
		  totalPayment+=unliPork;
		  String order2 = "Unli-Pork Fat + Sisig          : P180.00  \n";
		  orderCart+=order2;
		break;
		
		case 3: 
		  System.out.println("Bangus Sisig + Unli-Rice      : P180.00 added to cart");
		  totalPayment+=bangusSisig;
		  String order3 = "Bangus Sisig + Unli-Rice      : P180.00 \n";
		  orderCart+=order3;
		  
		break;
	      
	       default:
		 System.out.println("Enter valid entry only base on the choices above!");
		 
	       break;  
	      
	      }
	    

	  } else if(orderCategory == 2) {
	    System.out.println("==========WELCOME TO MANG KULAFS TAGAYAN! ========");
	    System.out.println("|***************ORDER BEVERAGE********************|");
	    System.out.println("| [1] 1-Bucket of Red Horse Stallion : P310.00    |");
	    System.out.println("| [2] 1-Tower of Beer na Beer Pilsen : P280.00    |");
	    System.out.println("| [3] Kulafu Special for Cult Members: P180.00    |");
	    System.out.println("| Enter the number for your choice below          |");
	    System.out.println("==================================================");
	    System.out.print  ("Choice:");
	    
	    float redhorse = 310 , bnbp = 280, kulafu = 180;
	    int orderChoice = console.nextInt();
	    
	      switch (orderChoice) {
		case 1: 
		  System.out.println("1-Bucket of Red Horse Stallion : P310.00 added to cart");
		  totalPayment+=redhorse;
		  String order1 = "1-Bucket of Red Horse Stallion : P310.00 \n";
		  orderCart+=order1;
		  
		  
		  
		  
		break;
		
		case 2: 
		  System.out.println("1-Tower of Beer na Beer Pilsen : P280.00 added to cart");
		  totalPayment+=bnbp;
		  String order2 = "1-Tower of Beer na Beer Pilsen : P280.00 \n";
		  orderCart+=order2;
		  
		  
		  
		break;
		
		case 3: 
		  System.out.println("Kulafu Special for Cult Members: P180.00  added to cart");
		  totalPayment+=kulafu;
		  String order3 = "Kulafu Special for Cult Members: P180.00 \n";
		  orderCart+=order3;
		  
		  
		break;
	      
	       default:
		 System.out.println("Enter valid entry only base on the choices above!");
	       break;  
	      
	      }
	    
	    
	    }
	    
	    else if(orderCategory == 3) {
	    System.out.println("==========WELCOME TO MANG KULAFS TAGAYAN! ========");
	    System.out.println("|*************ORDER SNACKS / PULUTAN*************|");
	    System.out.println("| [1] Chicken Skin in a plate       : P150.00    |");
	    System.out.println("| [2] Kropek Dragon Skin            : P180.00    |");
	    System.out.println("| [3] Kropek Vegatarian Special     : P120.00    |");
	    System.out.println("| Enter the number for your choice below         |");
	    System.out.println("==================================================");
	    System.out.print  ("Choice:");
	    
	    float chickenSkin = 150 , kropekDragon = 180, kropekVeg = 120;
	    int orderChoice = console.nextInt();
	    
	      switch (orderChoice) {
		case 1: 
		  System.out.println("Chicken Skin in a plate       : P150.00 added to cart");
		  totalPayment+=chickenSkin;
		  String order1 = "Chicken Skin in a plate       : P150.00 \n";
		  orderCart+=order1;
		break;
		
		case 2: 
		  System.out.println("Kropek Dragon Skin            : P180.00 added to cart");
		  totalPayment+=kropekDragon;
		  String order2 = "Kropek Dragon Skin            : P180.00 \n";
		  orderCart+=order2;
		break;
		
		case 3: 
		  System.out.println("Kropek Vegatarian Special     : P120.00  added to cart");
		  totalPayment+=kropekVeg;
		   String order3 = "Kropek Vegatarian Special     : P120.00 \n";
		   orderCart+=order3;
		  
		  
		break;
	      
	       default:
		 System.out.println("Enter valid entry only base on the choices above!");
		 
	       break;  
	      
	      }
	    
	    }
   }
   
   else {
   
   System.out.println("Okay! Have a nice day!~ ;)");
   System.exit(0);
   
   
   }
   
   
   
   
   System.out.println("Order again?");
   System.out.println("[1] - Yes");
   System.out.println("[2] - No");
   respondToOrder = console.nextInt();
   
    
  } while(respondToOrder == 1);
  
    System.out.println("Amount to pay: "+totalPayment);
    System.out.print("Enter cash payment: ");
    customerCash = console.nextFloat();
  
    System.out.println("==========R E C E I P T ========");
    System.out.println(orderCart);
     System.out.printf("TOTAL: %.2f\n",totalPayment);
    System.out.println("Change: " + (customerCash - totalPayment));
    System.out.println("================================");
     System.out.println("Thank you come again!");
  
  
  
  
  

  }


}
