import java.util.Random;
class RandomNumberThread extends Thread 
{
	public void run() 
	{
		Random random = new Random();
		for (int i = 0; i < 10; i++) 
		{
			int randomInteger = random.nextInt(100);
			System.out.println("Random Integer generated : " + randomInteger);
			if((randomInteger%2) == 0) 
			{
				SquareThread sThread = new SquareThread(randomInteger);
				sThread.start();
			}
			else
			 {
				CubeThread cThread = new CubeThread(randomInteger);
				cThread.start();
			}
			try 
			{
				Thread.sleep(1000);
			} 
			catch (InterruptedException ex) 
			{
				System.out.println(ex);
			}
		}
	}
}
class SquareThread extends Thread 
{
	int number;
	SquareThread(int randomNumbern) 
	{
		number = randomNumbern;
	}
	public void run() {
		System.out.println("Square of " + number + " = " + (number * number));
	}
}
class CubeThread extends Thread 
{
	int number;
	CubeThread(int randomNumber) 
	{
		number = randomNumber;
	}
	public void run() 
	{
		System.out.println("Cube of " + number + " = " + number * number * number);
	}
}
class MultiThreadingTest 
{
	public static void main(String args[]) 
	{
		RandomNumberThread rnThread = new RandomNumberThread();
		rnThread.start();
	}
}



OUTPUT:
Random Integer generated : 78
Square of 78 = 6084
Random Integer generated : 47
Cube of 47 = 103823
Random Integer generated : 1
Cube of 1 = 1
Random Integer generated : 18
Square of 18 = 324
Random Integer generated : 92
Square of 92 = 8464
Random Integer generated : 93
Cube of 93 = 804357
Random Integer generated : 63
Cube of 63 = 250047
Random Integer generated : 78
Square of 78 = 6084
Random Integer generated : 3
Cube of 3 = 27
Random Integer generated : 58
Square of 58 = 3364
