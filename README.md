# Java-program-to-find-out-the-quadrant-in-which-the-given-co-ordinate-lie

Quadrant in which the given co-ordinate lie
There are 2 axis (say x and y axis) in a two-dimensional planes. Based on values either positive or negative, a point is decided to lie on which co-ordinate. We need simple if-else statements to write a Java program to find out the quadrant in which the given co-ordinate lie. Generally there are four quadrants. 

Working :
According mathematics quadrants rules:

X  is positive integer as well as Y is also positive a integer it signifies first quadrant.
X  is negative integer but Y is positive integer it signifies second quadrant.
X  is negative integer as well as Y is also negative integer it signifies third quadrant.
X  is positive integer but Y is negative integer it signifies fourth quadrant.
Algorithm :
Get value of x & y
If ( x>0 and y>0 ) First Quadrant
If ( x<0 and y>0 ) Second Quadrant
If ( x<0 and y<0 ) Third Quadrant
If ( x>0 and y>0 ) Fourth Quadrant
If ( x=0 and y=0 ) Origin
If ( x!=0 and y=0 ) x-axis
If ( x>0 and y>0 ) y-axis
Quadrant in which Coordinate Lie
Java code
Run
import java.io.*;

public class Main
{

    public static void main (String[] args) 
    {

        int x=-3, y=-33;

        //find true condition of first quadrant
        if(x>0 && y>0)
            System.out.println("Quadrant I");   

        //find second quadrant
        else if(x<0 && y>0)
            System.out.println("Quadrant II");

        //To find third quadrant
        else if(x<0 && y<0) System.out.println("Quadrant III"); 

        //To find Fourth quadrant 
        else if (x > 0 && y < 0)
            System.out.println("Quadrant IV");
            
        //To find dose not lie on origin
        else if (x == 0 && y == 0)
            System.out.println("Origin");
            
        //On x-axis
        else if (y==0 && x!=0)
            System.out.println("x-axis");
            
        //On y-axis
        else if (x==0 && y!=0)
            System.out.println("y-axis");

    }
}
Output
Insert the value for variable X and Y : -3 -33
point (-3, -33) lies in the Third quadrant
