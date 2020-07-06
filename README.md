# Bubble-sort-in-java
in java


import java.util.*;
import java.io.*;
public class HelloWorld{

     public static void main(String []args)
     {
         Scanner sc=new Scanner(System.in);
         int n=sc.nextInt();
         int[] arr=new int[n];
         for(int i=0;i<n;i++)
         {
           arr[i]=sc.nextInt();   
        
         }
         int[] result=check(arr);
         for(int j=0;j<n;j++)
         {
         System.out.println(result[j]);
         }
        
     }
     static int[] check(int[] arr)
     {
        
         int p=0;
         for(int j=0;j<arr.length-1;j++)
         {
         for(int i=0;i<arr.length-j-1;i++)
         {
             int min=arr[i];
            
                 if(min>arr[i+1])
                 {
                     int temp=arr[i];
                     arr[i]=arr[i+1];
                     arr[i+1]=temp;  
                     
                 }
         }
         }
         return arr;
     }
}
