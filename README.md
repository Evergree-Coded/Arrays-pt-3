# Arrays pt 3

#### How to find the biggest/smallest element:
```java
int [] age = {55, 2, 5, 84, 27};
int smallest = age[0]; //temp var that stores the element at index 0
for(int i = 1; i < age.length; i++){
  if(age[i] < smallest){
    smallest = age[i];
  }
  //smallest = Math.min(age[i], smallest);
}
//Find Biggest
int [] age = {55, 2, 5, 84, 27};
int biggest = age[0]; //temp var that stores the element at index 0
for(int i = 1; i < age.length; i++){
  if(age[i] > biggest){
    biggest = age[i];
  }
  //smallest = Math.min(age[i], smallest);
}
```

#### Copy one array into another
```java
String [] groceryList = {"potatoes", "strawberry", "onions", "eggs"};
String [] transferList = new String[groceryList.length];
for(int i = 0; i < groceryList.length; i++){
  transferList[i] = groceryList[i];
}

```

#### Combine two arrays into one big array
```java
String [] groceryList = {"potatoes", "strawberry", "onions", "eggs"};
String [] additionalGroc = {"hot cheetos", "oreos", "dog food"};
String [] combinedList = new String[groceryList.length + additionalGroc.length];
for(int i = 0; i < groceryList.length; i++){
  combinedList[i] = groceryList[i];
}
for(int j = 0; j < additionalGroc.length; j++){
  combinedList[j + groceryList.length] = additionalGroc[j];
}

```
