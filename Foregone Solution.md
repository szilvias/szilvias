```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner input =  new Scanner(System.in);
        int T = input.nextInt();
        for (int k = 1; k <= T; k++){
            int N = input.nextInt(); 
            int temp = N;
            double b=0;
            int i = 0;
            while(N != 0){                
                if(N%10 == 4){
                    b = b + Math.pow(10, i);
                }
                i=i+1;
                N = N/10;
            }
            int B = (int) b;
            int A = temp - B;           
            System.out.println("Case #" + k +": " + A + " " + B);
        }
    }    
}
```
Set 1 and Set 2 passed
Set 3 RE 
