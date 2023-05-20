VB.NET
Q1Write a Vb.net program for blinking an image
Program:- 
Public Class slip2

    Private Sub Timer1_Tick(sender As Object, e As EventArgs) Handles Timer1.Tick

        PictureBox1.Visible = Not PictureBox1.Visible

    End Sub

End Class

Design:- 

1) Get  Picturbox and timer control on design form.

2) Make timer control Enabled=True 

3) Insert image on Picturebox 

4) To fit the image PictureBox set Sizemode property to StretchImage


...............///////////.........../////////........///////////.......///////////
Q2
.......////////
// C# program to create marksheet for students.
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

class GFG{
	
static void Main(string[] args)
{
	
	
	int r, marks1, marks2, marks3, total;
	
	
	float percentage;
	string n;
	
	Console.WriteLine("Enter Student Roll Number :");
	r = Convert.ToInt32(Console.ReadLine());
	
	Console.WriteLine("Enter Student Name :");
	n = Console.ReadLine();
	
	Console.WriteLine("Enter Subject-1 Marks : ");
	marks1 = Convert.ToInt32(Console.ReadLine());
	
	Console.WriteLine("Enter Subject-2 Marks : ");
	marks2 = Convert.ToInt32(Console.ReadLine());
	

	Console.WriteLine("Enter Subject-3 Marks :");
	marks3 = Convert.ToInt32(Console.ReadLine());
	
	total = marks1 + marks2 + marks3;
	
	percentage = total / 3.0f;
	

	Console.WriteLine("Final result of {0} is:", n);
	Console.WriteLine("Total Marks : " + total);
	Console.WriteLine("Percentage : " + percentage);
	
	// Calculate grades
	if (percentage <= 35)
	{
		Console.WriteLine("Grade is F");
		Console.ReadLine();
	}
	else if (percentage >= 34 && percentage <= 39)
	{
		Console.WriteLine("Grade is D");
	}
	else if (percentage >= 40 && percentage <= 59)
	{
		Console.WriteLine("Grade is C");
	}
	else if (percentage >= 60 && percentage <= 69)
	{
		Console.WriteLine("Grade is B");
	}
	else if (percentage >= 70 && percentage <= 79)
	{
		Console.WriteLine("Grade is B+");
	}
	else if (percentage >= 80 && percentage <= 90)
	{
		Console.WriteLine("Grade is A");
	}
	else if (percentage >= 91)
	{
		Console.WriteLine("Grade is A+");
	}
}
}

.......///////...../////////.........//////////////...........///////////..........///////////
Q1 java
	.......................
public class Demo extends Thread{
public void run(){
for (int i = 0; i < 5; i++) {
System.out.println("The Thread name is " + Thread.currentThread().getName());
}
}
public static void main(String[] args) {
Demo t1 = new Demo();
t1.setName("Main Thread");
t1.start();
Thread t2 = currentThread();
t2.setName("Current Thread");
for (int i = 0; i < 5; i++) {
System.out.println("The Thread name is " + t1.currentThread().getName());
}
}
}

.......///////...../////////.........//////////////...........///////////..........///////////
Q2
.......
import ="java.sql.*"
<html>
<head>
<title>College Details</title>
</head>
<body>
<h1>College Details</h1>
<table border="1">
<tr>
<th>College ID</th>
<th>College Name</th>
<th>Address</th>
</tr>
<%
try{
Class.forName("com.mysql.jdbc.Driver");
Connection con =DriverManager.getConnection("jdbc:mysql://localhost:3306/collegedb","root", "password");
Statement stmt = con.createStatement();
ResultSet rs = stmt.executeQuery("SELECT CollegeID, Coll_Name, Address
FROM College");
while (rs.next()) {
%>
<tr>
<td><%= rs.getString("CollegeID") %></td>
<td><%= rs.getString("Coll_Name") %></td>
<td><%= rs.getString("Address") %></td>
</tr>
<%
}
rs.close();
stmt.close();
con.close();
} catch (Exception e) {
out.println("Error: " + e.getMessage());
}
%>
</table>
</body>
</html>
	
.............//////////////.............////////////............/////////////.......////////////////

