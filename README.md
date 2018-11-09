# BadProductsArray
BadProductsArray
public class BadProductsArray {

public static void main(String[] args) {
	 
	int[] arr= {1,1,1,1,0};
	boolean bool=badP(arr, 1);
	System.out.println(bool);
}

  public static boolean badP(int[] products, int limit){
	
	  int countOfZero=0; 
   for(int z=0; z<products.length; z++) {
	   if(products[z]==0) {
	   countOfZero++;
	   }
  } if(countOfZero<limit) {
   return true;
  } else {
	   return false;
  }	  
  }
}

