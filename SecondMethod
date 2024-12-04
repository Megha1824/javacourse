package com.anpc9531.day18;

import java.util.Scanner;

class Demo8 implements Runnable
{
	public void run()
	{
		Thread t = Thread.currentThread();
		String name = t.getName();
		if(name.equals("ADD")==true)
		{
			add();
		}
		else if(name.equals("CHAR")==true)
		{
			charPrint();
		}
		else
		{
			numPrint();
		}
	}
	
	void add()
	{
		System.out.println("Addition task started");
		Scanner s = new Scanner(System.in);
		
		System.out.println("Enter the first number");
		int a = s.nextInt();
		System.out.println("Enter the second number");
		int b = s.nextInt();
	    int c = a+b;
		System.out.println(c);
		System.out.println("Addition task completed");
	}
	void charPrint()
	{
		System.out.println("Character printing task started");
		for(int i = 65 ; i<=75 ; i++)
		{
			System.out.println((char)i);
			try {
			Thread.sleep(4000);
			}
			catch(Exception e)
			{
				System.out.println("Some problem occured");
			}
		}
		System.out.println("Character printing task completed");
	}
	void numPrint()
	{
		System.out.println("Number printing task started");
		for(int i =1;i<=10;i++)
		{
			System.out.println(i);
			try {
			Thread.sleep(4000);
			}
			catch(Exception e)
			{
				System.out.println("Some problem occurred");
			}
		}
		System.out.println("Number printing task completed");
	}
}

public class SecondMethod {

	public static void main(String[] args) {
		
		Demo8 d1 = new Demo8();
		
		Thread t1 = new Thread(d1);
		Thread t2 = new Thread(d1);
		Thread t3 = new Thread(d1);
		
		t1.setName("ADD");
		t2.setName("CHAR");
		t3.setName("NUM");
		
		t1.start();
		t2.start();
		t3.start();
		
	}

}
