## Note
```
Comparator is an interface 
The array.sort() method will sort based on Asscending or descending order but using comparator we can able to sort in a cutomized way
e.g can sort based on the string length 

Two objects can be compared using .equals() 
e.g obj1.equals(obj2); -> this will give the boolean vale True / False but wont tell which is smaller and greater
```
## Return
```
obj1 > obj2 = +ve no
obj1 < obj2 = -ve no
obj1 = obj2 = 0
```

## Exception 
```
if it cant compare the any two objects then it will throw classcast exception
```
## Statement
```
Write a program to sort objects length using comparator interface 
```
## Sample input
```
"Samdany","Jamescastro","George","xavier"
```

## Code
```

class Comaparatordemo implements Comparator{

	@Override
	public int compare(Object o1, Object o2) {
        //type casting the object
		String s1 = (String)o1;
		String s2 = (String)o2;
		if(s1.length() > s2.length()) 
			return +1;
		else if(s1.length() < s2.length())
		    return -1;
		else 
			return 0;
		
	}
	
}

public class Revs {
    
	public static void main(String[] args) {
	  String[] names = {"Samdany","Jamescastro","George","xavier"};
	  Comparator comp = new Comaparatordemo();
	  Arrays.sort(names,comp);
	  for(String i: names)
	  System.out.println(i);
	}
	
}
```
## output
```
George
xavier
Samdany
Jamescastro
```

