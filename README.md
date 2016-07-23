# armstrongnumber
import java.util.Scanner;
public class Codekata1 {
	static Scanner ab=new Scanner(System.in);
	public static void main(String[]arg){
		int num;
		int y,b;
		int count=0;
		int sum=0;
		int x;
	System.out.println("enter the number");
	
	num=ab.nextInt();
	

	int [] u=new int[100000];
	for(int i=0;i<num;i++)
	{
		u[i]=num%10;
		num=num/10;
		count++;
	}
	
	int z=count;
	
	
	for(int i=0;i<z;i++)
		
	{
		
		u[i]=(int) Math.pow(u[i],z);
		sum=sum+u[i];
	}
	System.out.println(sum);
}
	
}
