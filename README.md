# 23.09.22
## 1. This kata is about multiplying a given number by eight if it is an even number and by nine otherwise.
___
### Мое рещение 
```java
public class Sid {
    public static int simpleMultiplication(int n) {
        if (n % 2 == 0) {
        return n * 8;
         } else {
         return n * 9;
        }
    }
}
```

### Понравившееся решение
```java
public class Sid {
    public static int simpleMultiplication (int n) {
        return n % 2 == 0 ? n * 8 : n * 9;
    }
}
```
## 2.Consider an array/list of sheep where some sheep may be missing from their place. We need a function that counts the number of sheep present in the array (true means present).
### Мое рещение 
```java
public class Counter {
  public int countSheeps(Boolean[] arrayOfSheeps) {
    int sumOfSheep = 0;
    for(Boolean sheep:arrayOfSheeps){
      if(sheep == Boolean.TRUE){
        sumOfSheep++;
      }
      else if(sheep == null){
        continue;
      }
    }
    return sumOfSheep;
  }
}
```

### Понравившееся решение
```java
public class Counter {
  public int countSheeps(Boolean[] arrayOfSheeps) {
    int counter = 0;
    for (Boolean present : arrayOfSheeps) {
      if (present != null && present) {
        counter += 1;
      }
    }
    return counter;
  }
}
```
