# Arrays
There are two types of arrays as follows:

## 1. Single Dimensional Array
Single dimensional consists of the 1D array. It may have a single row or a single column.

We can declare a single dimensional array as below:
```java
int[] a; 
OR 
int a[]; 
OR 
int []a; 
OR 
int[]a;

But the most preferred way is int[] a;
```

`Note: At the time of declaration we are not proving the size of the Array.`

**Declaration of array**
```java
int[] a; //Declaration of the array
```

**Creation of array**
```java
a = new int[5] //Creation of array
```

`Note: At the time of array creation, providing the size of an array is very important.`

**Declaration and creation of array in a single line** 
```java
int[] a = new int[3];       //Declare, create
```


**Initialize the array**

- Add some values in an array
```java
a[0] = 1; // We are adding 1 at 0th position in array.  
a[1] =2;  
a[2] =3;
```

`Note:  If I gave the index no, which does not exist on the array, it throws an ArrayIndexLoutOfBoundException. You cannot add values beyond the size of an array.`

**Declaration, creation and initialization of array in a single line** 
```java
int[] a = {1,2,3,4,5};     //Declare, create, initialize
OR
int[] a =  new int[] {1,2,3,4,5};
```

**Retrieve elements from a single-dimensional array:**
```java
public class Demo{  
public static void main (String args[])

 { 
 int[] a = new int[] {1,2,3,4,5}; 
 for(int i=0; i<=a.length-1;i++) 
 { 
 System.out.println(a[i]); 
 }  }  }
```
Output
```
1
2
3
4
5
```



## 2. Multi-Dimensional Array
The multi-dimensional array is basically array of arrays (aka jagged arrays).

**Declaration of the array**
```java
int [][] a; //here we declared array a
```

**Creation of array**
```java
a = new int[2][4];
```

**Initialize the array**
```java
a[0][0] = 10  
a[0][1] = 20  
a[0][2] = 30 
a[0][3] = 40
```

**Declaration and creation of array in a single line** 
```java
int[][] a =new int[2][3];
```

**Declaration, creation and initialization of array in a single line** 
```java
int[][] a = {{10,20,30},{100,200,300}};
```

**Code:** (taking user input and print)
```java
import java.util.Scanner;  
public class InsArray{  
public static void main(String[] args)  
{  
int[][] twodArray = new int[3][2]; // declared and created array object  
Scanner s1 = new Scanner(System.in); //created Scanner object
	
System.out.println("Please enter the values to be added");  
	
for(int i = 0 ; i < 3 ; i++)
{  
	for(int j = 0 ; j < 2; j++)  
	{  
		twodArray[i][j] = s1.nextInt();  
	}  
	System.out.println();  
}  
	
System.out.println("Your output would be as below:");
	
for(int i = 0 ; i < 3 ; i++)
{  
	for(int j = 0 ; j < 2; j++)  
	{  
		System.out.print(twodArray[i][j] + " " );  
	}  
	System.out.println();  
}  
}
}

```
Output:
```
Please enter the values to be added

22  
11  
22  
33  
44  
55

Your output would be as below:

22 11  
22 33  
44 55
```

**Code 2** (Update Elements of 2D Arrays in Java)
```java
public class UpArray{  
public static void main (String[] args)  
{  
String[][] twoDimentional = {{"1","1"},{"2","2"},{"3","3"},{"4","4"}};  
System.out.println("Before updating an array: ");  
printArray(twoDimentional);  
twoDimentional[3][0] = "5";  
System.out.println("After updating an array element: ");  
printArray(twoDimentional);  
} 
	
private static void printArray(String[][] twoDimentional){  
for(int i=0; i<twoDimentional.length; i++)
{  
	for(int j=0; j<twoDimentional[0].length; j++)
	{  
		System.out.print(twoDimentional[i][j]);  
	}  
System.out.println("");  
}  
}  
}
```
Output:
```
Before updating an array:
11
22
33
44
After updating an array element:
11
22
33
54
```
