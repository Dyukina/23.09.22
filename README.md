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
## 2.
