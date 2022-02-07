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
public class Demo2{  
public static void main (String args[])
{  
int[] a =  new int[] {1,2,3,4,5};  
for(int i=0; i<=a.length-1;i++)  
{  
System.out.println(a[i]);  
}  }  }
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

**Code:**
```java
public class MyArray {  
public static void main(String[] args)  
{  
int[][] a = {{10,20,30},{100,200,300}};  
System.out.print(a[1][2]);  
}  
}
```
