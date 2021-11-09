import java.util.*;

public class Main {  
    public static void main(String[] args) {  
        Scanner sc = new Scanner(System.in);  
        int n = sc.nextInt();  
        int[] a = new int[n];  
        int tmp;  
       
        for(int i = 0; i < n; i++){  
             a[i] = sc.nextInt();  
        }  
        
            for(int j = 0; j < n-1; j++){  
                for(int k = j+1; k < n; k++){  
                    if(a[j] > a[k]){  
                    tmp = a[j];  
                    a[j] = a[k];  
                    a[k] = tmp ;  
                    }  
                }  
            }  
            
        for(int i = 0; i < n; i++){  
        System.out.println(a[i]);  
        }  
    }  
}  
