# hello-world
package practice;

import java.util.Arrays;

public class removedup {

	public static void main(String[] args) {
		int a[]= {1,2,3,4,1,3,2};
		int cnt=0;
		for (int i = 0; i < a.length; i++)
		{
			for (int j = i+1; j < a.length; j++)
			{
				if(a[i]==a[j])
				{
					cnt++;
					break;
				}
				
			}
		}
		System.out.println(cnt);
		int b[]=new int[a.length-cnt];
		int rem=0;
		for (int i = 0; i < a.length; i++)
		{
			cnt=0;
			for (int j = 0; j < b.length; j++)
			{
				if(a[i]==b[j])
				{
					cnt++;
					break;
				}
			}
			if(cnt==0)
			{
				b[rem++]=a[i];
			}
		}
		System.out.println(Arrays.toString(b));

	}

}
JAVA
