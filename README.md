# currency-conversion
import java.util.*;
import java.text.DecimalFormat;

 // Compiler version JDK 11.0.2

 class  currency
 { 
   public static void main(String args[])
   { double rupees, code, dollar;
    DecimalFormat f = new DecimalFormat("##.###");
   Scanner in=new Scanner(System.in);
    System.out.println("enter currency code 1:CAD\n2: HKD\n3:SGD\n4:USD");
  code=in.nextInt();
  
  if(code == 1)
  {
    System.out.println("enter dollar");
    dollar=in.nextFloat();
    
    rupees=dollar*52.08;
    System.out.println("CAD is"+ dollar +  " rupees is "+f.format(rupees));
  }
 else if(code == 2)
  {
    System.out.println("enter dollar");
    dollar=in.nextFloat();
    
    rupees=dollar*8.86;
    System.out.println("HKD is"+ dollar + " rupees is "+f.format(rupees));
  }
 else if(code == 3)
  {
    System.out.println("enter dollar");
    dollar=in.nextFloat();
    
    rupees=dollar*51.29;
    System.out.println(" SGD is"+ dollar + " rupees is "+f.format(rupees));
  }
 else if(code == 4)
  {
    System.out.println("enter dollar");
    dollar=in.nextFloat();
    
    rupees=dollar*69.55;
    System.out.println("USD is"+ dollar + " rupees is "+f.format(rupees));
  }
  else
  {
    System.out.println("invalid input");
  }
  
   }
 }
