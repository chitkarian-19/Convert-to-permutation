# Convert-to-permutation
Starters 69 | Convert to permutation

```cpp
/* package codechef; // don't place package name! */

import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		Scanner sc = new Scanner(System.in);
		int t=sc.nextInt();
		StringBuilder op=new StringBuilder("");
		
		while(t-->0){
		    int n = sc.nextInt();
		    int[] a = new int[n];
		    int flag = 0;
		    
		    for(int i=0;i<n;i++){
		        a[i]=sc.nextInt();
		    }
		    Arrays.sort(a);
		    int outp = 0;
		    for(int i=0;i<n;i++){
		        if(a[i]>(i+1)){
		            outp=-1;
		            break;
		        }
		        else{
		            outp=outp+((i+1)-a[i]);
		        }
		    }
		    
		    op.append(outp+"\n");
		    
		
	}
	
	    System.out.print(op.toString());
	}
}

```
