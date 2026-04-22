# Loop Practice 20 – Questions, Code & Explanation


## 1. Print numbers from 1 to 20

### Description

Print numbers starting from 1 up to 10 using a loop.

### Code

```java
public class Q1 {
    public static void main(String[] args) {
        for (int i = 1; i <= 10; i++) {
            System.out.println(i);
        }
    }
}
```

### Explanation

* Loop starts at 1 and runs until 10
* `i++` increments the value each time

---

## 2. Print numbers from 10 to 1

### Description

Print numbers in reverse order.

### Code

```java
public class Q2 {
    public static void main(String[] args) {
        for (int i = 10; i >= 1; i--) {
            System.out.println(i);
        }
    }
}
```

### Explanation

* Loop starts from 10
* Decreases using `i--`

---

## 3. Print even numbers from 1 to 20

### Description

Display all even numbers between 1 and 20.

### Code

```java
public class Q3 {
    public static void main(String[] args) {
        for (int i = 2; i <= 20; i += 2) {
            System.out.println(i);
        }
    }
}
```

### Explanation

* Starts at 2 (first even number)
* Increments by 2

---

## 4. Print odd numbers from 1 to 20

### Description

Display all odd numbers between 1 and 20.

### Code

```java
public class Q4 {
    public static void main(String[] args) {
        for (int i = 1; i <= 20; i += 2) {
            System.out.println(i);
        }
    }
}
```

---

## 5. Sum of first 10 natural numbers

### Description

Calculate the sum of numbers from 1 to 10.

### Code

```java
public class Q5 {
    public static void main(String[] args) {
        int sum = 0;
        for (int i = 1; i <= 10; i++) {
            sum += i;
        }
        System.out.println(sum);
    }
}
```

### Explanation

* `sum += i` adds each number
* Final result is 55

---

## 6. Factorial of a number

### Description

Find factorial of a number (e.g., 5! = 120).

### Code

```java
public class Q6 {
    public static void main(String[] args) {
        int num = 5, fact = 1;

        for (int i = 1; i <= num; i++) {
            fact *= i;
        }

        System.out.println(fact);
    }
}
```

### Explanation

* Multiply numbers from 1 to n
* `fact *= i` builds factorial

---

## 7. Multiplication table

### Description

Print multiplication table of a number.

### Code

```java
public class Q7 {
    public static void main(String[] args) {
        int num = 5;

        for (int i = 1; i <= 10; i++) {
            System.out.println(num + " x " + i + " = " + (num * i));
        }
    }
}
```

---

## 8. Reverse a number

### Description

Reverse digits of a number.

### Code

```java
public class Q8 {
    public static void main(String[] args) {
        int num = 1234, rev = 0;

        while (num != 0) {
            rev = rev * 10 + num % 10;
            num /= 10;
        }

        System.out.println(rev);
    }
}
```

### Explanation

* Extract digit using `% 10`
* Build reverse number

---

## 9. Count digits in a number

### Description

Count total digits in a number.

### Code

```java
public class Q9 {
    public static void main(String[] args) {
        int num = 12345, count = 0;

        while (num != 0) {
            count++;
            num /= 10;
        }

        System.out.println(count);
    }
}
```

---

## 10. Sum of digits

### Description

Find sum of digits of a number.

### Code

```java
public class Q10 {
    public static void main(String[] args) {
        int num = 123, sum = 0;

        while (num != 0) {
            sum += num % 10;
            num /= 10;
        }

        System.out.println(sum);
    }
}
```

---

## 11. Palindrome number

### Description

Check if a number reads same forward and backward.

### Code

```java
public class Q11 {
    public static void main(String[] args) {
        int num = 121, temp = num, rev = 0;

        while (num != 0) {
            rev = rev * 10 + num % 10;
            num /= 10;
        }

        if (temp == rev)
            System.out.println("Palindrome");
        else
            System.out.println("Not Palindrome");
    }
}
```

---

## 12. Check prime number

### Description

Check if number is divisible only by 1 and itself.

### Code

```java
public class Q12 {
    public static void main(String[] args) {
        int num = 7;
        boolean isPrime = true;

        for (int i = 2; i <= num / 2; i++) {
            if (num % i == 0) {
                isPrime = false;
                break;
            }
        }

        System.out.println(isPrime ? "Prime" : "Not Prime");
    }
}
```

---

## 13. Fibonacci series

### Description

Print first 10 Fibonacci numbers.

### Code

```java
public class Q13 {
    public static void main(String[] args) {
        int a = 0, b = 1;

        for (int i = 1; i <= 10; i++) {
            System.out.println(a);
            int c = a + b;
            a = b;
            b = c;
        }
    }
}
```

---

## 14. Print square numbers

### Description

Print squares of numbers from 1 to 10.

### Code

```java
public class Q14 {
    public static void main(String[] args) {
        for (int i = 1; i <= 10; i++) {
            System.out.println(i * i);
        }
    }
}
```

---

## 15. Print cube numbers

### Description

Print cubes of numbers from 1 to 10.

### Code

```java
public class Q15 {
    public static void main(String[] args) {
        for (int i = 1; i <= 10; i++) {
            System.out.println(i * i * i);
        }
    }
}
```

---

## 16. Sum of even numbers

### Description

Find sum of even numbers from 1 to 20.

### Code

```java
public class Q16 {
    public static void main(String[] args) {
        int sum = 0;

        for (int i = 2; i <= 20; i += 2) {
            sum += i;
        }

        System.out.println(sum);
    }
}
```

---

## 17. Sum of odd numbers

### Description

Find sum of odd numbers from 1 to 20.

### Code

```java
public class Q17 {
    public static void main(String[] args) {
        int sum = 0;

        for (int i = 1; i <= 20; i += 2) {
            sum += i;
        }

        System.out.println(sum);
    }
}
```

---

## 18. Find largest digit in number

### Description

Find the biggest digit in a number.

### Code

```java
public class Q18 {
    public static void main(String[] args) {
        int num = 593, max = 0;

        while (num != 0) {
            int digit = num % 10;

            if (digit > max) {
                max = digit;
            }

            num /= 10;
        }

        System.out.println(max);
    }
}
```

---

## 19. Star pattern (increasing)

### Description

Print triangle star pattern.

### Code

```java
public class Q19 {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

---

## 20. Star pattern (decreasing)

### Description

Print reverse triangle pattern.

### Code

```java
public class Q20 {
    public static void main(String[] args) {
        for (int i = 5; i >= 1; i--) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```
