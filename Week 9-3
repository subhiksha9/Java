import java.util.*;
class NumberException
{
	public static void main(String args[])
	{
		int a;
		try
		{
			Scanner sc=new Scanner(System.in);
			System.out.print("Enter a number :");
			a=sc.nextInt();
			if(a<10 || a>50)
			{
				throw new Exception("OutOfRangeException");
			}
			else
			{
				System.out.println("Square of "+a+" = "+(a*a));
			}
		}
		catch(Exception e)
		{
			System.out.println(e);
		}
	}
}
