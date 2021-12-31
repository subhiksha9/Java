package p1;
public class Protection
{
	int n=10;                        //variable declare as default
	private int n_pri=20;     //variable declare as private
	protected int n_pro=30;    //variable declare as protected
	public int n_pub=40;     //variable declare as public
	public Protection()
	{
		System.out.println("Base Class in package p1:");
		System.out.println("Defalut Variable n: "+n);
		System.out.println("Private Variable n_pri: "+n_pri);
		System.out.println("Protected Variable n_pro: "+n_pro);
		System.out.println("Public Variable n_pub: "+n_pub);
	}
}

package p1;
public class Derived extends Protection
{
	public Derived()
	{
		System.out.println("Sub Class in same package p1:");
		System.out.println("Defalut Variable n: "+n);
		//private variable cannot accessed in sub class
		//System.out.println("Private Variable n_pri: "+n_pri);
		System.out.println("Protected Variable n_pro: "+n_pro);
		System.out.println("Public Variable n_pub: "+n_pub);
	}
}

package p1;
public class SamePackage
{
	public SamePackage()
	{
		Protection p = new Protection();

		System.out.println("SamePackage non sub Class in package p1:");
		System.out.println("Defalut Variable n: "+p.n);
		//private variable cannot accessed in same package non sub class
		//System.out.println("Private Variable n_pri: "+p.n_pri);
		System.out.println("Protected Variable n_pro: "+p.n_pro);
		System.out.println("Public Variable n_pub: "+p.n_pub);
	}
}

package p2;
public class Protection2 extends p1.Protection
{
	public Protection2()
	{
		System.out.println("Sub Class but different package p2:");
		//Default variable cannot accessed in different package and sub class
		//System.out.println("Defalut Variable n: "+n);
		//private variable cannot accessed in different package and sub class
		//System.out.println("Private Variable n_pri: "+n_pri);
		System.out.println("Protected Variable n_pro: "+n_pro);
		System.out.println("Public Variable n_pub: "+n_pub);
	}
}


package p2;
public class OtherPackage
{
	public OtherPackage()
	{
		p1.Protection p = new p1.Protection();
		System.out.println("Non Sub Class and different package p2:");
		//Default variable cannot accessed in different package and non sub class
		//System.out.println("Defalut Variable n: "+p.n);
		//private variable cannot accessed in different package and non sub class
		//System.out.println("Private Variable n_pri: "+p.n_pri);
		//protected variable cannot accessed in different package and non sub class
		//System.out.println("Protected Variable n_pro: "+p.n_pro);
		System.out.println("Public Variable n_pub: "+p.n_pub);
	}
}

package p1;
public class Test1
{
	public static void main(String args[])
	{
		Protection p=new Protection();
		System.out.println();
		Derived d=new Derived();
		System.out.println();
		SamePackage s=new SamePackage();	
	}
}

package p2;
public class Test2
{
	public static void main(String args[])
	{
		Protection2 p=new Protection2();
		System.out.println();
		OtherPackage d=new OtherPackage();	
	}
}
