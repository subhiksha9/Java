class CommandLine
{
	public static void main(String args[])
	{
		try
		{
			if(args.length==0)
			{
				throw new Exception("NoCommandLineArguments");
			}
			else
			{
				try
				{
					int a=Integer.valueOf(args[0]);
					int b=Integer.valueOf(args[1]);
					int c=a/b;
					System.out.println("a/b = "+c);
				}
				catch(ArithmeticException e)
				{
					System.out.println(e);
				}
			}
		}
		catch(Exception e)
		{
			System.out.println(e);
		}
	}
}
