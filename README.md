class Main {
    public static void main(String[] args) {
        
        String str= "mom";
        boolean b= new StringBuilder(str).reverse().toString().equals(str);
     
        System.out.println("This is a palinadrom string: " + b);
    }
}
OUTPUT: This is a palinadrom string: TRUE

--------------------------------------------------------------------------------------------------------------------------------------------
class Main {
    public static void main(String[] args) {
    
        
        String str= "time";
       String b = new StringBuilder(str).reverse().toString();
     
        System.out.println("This is a reversing a string: " + b);
    }
}
OUTPUT: This is a reversing a string: emit

--------------------------------------------------------------------------------------------------------------------------------------------
class Main {
    public static void main(String[] args) {
    
        
        String str= "Harshith@1325Hm";
       String remove = str.replaceAll("[a-z0-1]","");
     
        System.out.println("This is to remove letter from given string: " + remove);
    }
}
OUTPUT: This is to remove letter from given string: H@325H

--------------------------------------------------------------------------------------------------------------------------------------------
class Main {
    public static void main(String[] args) {
          
      int n=17;
      boolean b=true;
        
      for(int i=1;i<=n;i++){
            if(n%i==0){
                b=false;
            }
        }    
        System.out.println(n + " is a Prime number: " + b);
    }
}
OUTPUT: 17 is a Prime number: false

--------------------------------------------------------------------------------------------------------------------------------------------
class Main {
    public static void main(String[] args) {
          
     int i,fact=1,num=6;

        for(i=1;i<=num;i++){
            fact=fact*i;
        }
        System.out.println("Factorial of " + num + " is: " + fact );
    }
}
OUTPUT: Factorial of 6 is:720

--------------------------------------------------------------------------------------------------------------------------------------------
class Main {
    public static void main(String[] args) {
    
        String str="harshitha7733";
        String res="";

        for(int i=0;i<str.length();i++){
            char c= str.charAt(i);
            if(res.indexOf(c) == -1){
                res += c;            
            }
        }
     
        System.out.println("Unique letters from the string are :" + res);
    }
}
OUTPUT: Unique letters from the string are :harsit73

--------------------------------------------------------------------------------------------------------------------------------------------
class Main {
    public static void main(String[] args) {
        
         int n=7;
        if(n%2==0){
             System.out.println("Given number is Even");
        }else{
             System.out.println("Given number is Odd");
        }       
    }
}
OUTPUT: Given number is Odd

--------------------------------------------------------------------------------------------------------------------------------------------
import java.util.ArrayList;
import java.util.Collections;

class Main {
    public static void main(String[] args) {
        
     ArrayList<Integer> list=new ArrayList<>();
        list.add(2);
        list.add(88);
        list.add(6);

        int max= Collections.max(list);      
        System.out.println("Largest number is "+max);      
    }
}
OUTPUT: Largest number is 88

--------------------------------------------------------------------------------------------------------------------------------------------
 import java.util.Arrays;

class Main {
    public static void main(String[] args) {


        int arr[]={33,7,22,8,55};
        Arrays.sort(arr);
        System.out.println("Ascending Order: " + Arrays.toString(arr));  
        
        int max=arr[arr.length-1];
        System.out.println("Big number is : " + max);      
       
    }
}
UTPUT: Ascending Order: [7, 8, 22, 33, 55]
Big number is : 55

--------------------------------------------------------------------------------------------------------------------------------------------
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class Main {
    public static void main(String[] args) {

        WebDriver driver = new ChromeDriver();
        driver.manage().window().maximize();
        driver.get("https://www.flipkart.com");      
        System.out.println(driver.getTitle());    
        driver.quit();
       
    }
}
OUTPUT: Maximize window, open URL, print title, and close

--------------------------------------------------------------------------------------------------------------------------------------------
import {test, expect} from '@playwright';

    test('Verify google page title', async({page}) => {
    await page.goto('https://www.google.com');
    await expect(page).toHaveTitle(/google/);       
    });
OUTPUT: Playwright with typescript

---------------------------------------------------------------------------------------------------------------------------------------------- 
