## 🟢 LEVEL-1: SUPER BASIC (Must-Know)

1. Even / Odd
2. Positive / Negative / Zero
3. Prime Number
4. Odd numbers between 1–100
5. Even numbers between 1–100
6. Sum of first N numbers
7. Factorial
8. Fibonacci series
9. Reverse a number
10. Sum of digits
11. Count digits
12. Leap year
13. Multiplication table
14. Greatest of 2 numbers
15. Greatest of 3 numbers

---

## 1️⃣ Even / Odd (n = 4)

```python
n = 4
print("Even" if n % 2 == 0 else "Odd")
```

| Step | n | n % 2 |
| ---- | - | ----- |
| 1    | 4 | 0     |

**Result:** Even
**Bro Explain:** 2 se pura divide → Even

---

## 2️⃣ Positive / Negative (n = -5)

```python
n = -5
print("Positive" if n>0 else "Negative")
```

| Step | n  | n>0   |
| ---- | -- | ----- |
| 1    | -5 | False |

**Result:** Negative
**Bro Explain:** 0 se chhota → Negative

---

## 3️⃣ Prime Number (n = 7)

```python
n = 7
for i in range(2,n):
    if n % i == 0:
        print("Not Prime")
        break
else:
    print("Prime")
```

| i | 7 % i |
| - | ----- |
| 2 | 1     |
| 3 | 1     |
| 4 | 3     |
| 5 | 2     |
| 6 | 1     |

**Result:** Prime
**Bro Explain:** Kisi se divide nahi hua → Prime

---

## 4️⃣ Factorial (n = 5)

```python
n = 5
fact = 1
for i in range(1,n+1):
    fact *= i
print(fact)
```

| i | fact |
| - | ---- |
| 1 | 1    |
| 2 | 2    |
| 3 | 6    |
| 4 | 24   |
| 5 | 120  |

**Result:** 120
**Bro Explain:** Har step me purana × next

---

## 5️⃣ Fibonacci (n = 5)

```python
n = 5
a,b = 0,1
for _ in range(n):
    print(a, end=" ")
    a,b = b,a+b
```

| Step | a | b |
| ---- | - | - |
| 1    | 0 | 1 |
| 2    | 1 | 1 |
| 3    | 1 | 2 |
| 4    | 2 | 3 |
| 5    | 3 | 5 |

**Output:** 0 1 1 2 3
**Bro Explain:** Last 2 numbers add → next

---

## 6️⃣ Reverse Number (n = 123)

```python
n = 123
rev = 0
while n>0:
    rev = rev*10 + n%10
    n//=10
print(rev)
```

| Step | n   | rev |
| ---- | --- | --- |
| 1    | 123 | 3   |
| 2    | 12  | 32  |
| 3    | 1   | 321 |

**Result:** 321
**Bro Explain:** Peeche ka digit aage chipka

---

## 7️⃣ Palindrome (n = 121)

```python
n = 121
temp = n
rev = 0
while n>0:
    rev = rev*10 + n%10
    n//=10
print("Palindrome" if rev==temp else "Not Palindrome")
```

| Step | n   | rev |
| ---- | --- | --- |
| 1    | 121 | 1   |
| 2    | 12  | 12  |
| 3    | 1   | 121 |

**Result:** Palindrome
**Bro Explain:** Ulta = original → Palindrome

---

## 8️⃣ Armstrong (n = 153)

```python
n = 153
temp = n
sum = 0
while n>0:
    d = n%10
    sum += d**3
    n//=10
print("Armstrong" if sum==temp else "Not Armstrong")
```

| Digit | Cube | Sum |
| ----- | ---- | --- |
| 3     | 27   | 27  |
| 5     | 125  | 152 |
| 1     | 1    | 153 |

**Result:** Armstrong
**Bro Explain:** Digit³ ka sum = original

---

## 9️⃣ Sum of Digits (n = 123)

```python
n = 123
s = 0
while n>0:
    s += n%10
    n//=10
print(s)
```

| Digit | Sum |
| ----- | --- |
| 3     | 3   |
| 2     | 5   |
| 1     | 6   |

**Result:** 6
**Bro Explain:** Sab digits add

---

## 🔟 Count Digits (n = 4567)

```python
n = 4567
count = 0
while n>0:
    count+=1
    n//=10
print(count)
```

| Step | n   | count |
| ---- | --- | ----- |
| 1    | 456 | 1     |
| 2    | 45  | 2     |
| 3    | 4   | 3     |
| 4    | 0   | 4     |

**Result:** 4
**Bro Explain:** Har divide → count++

---

## 1️⃣1️⃣ Leap Year (2024)

```python
y = 2024
print("Leap Year" if y%400==0 or (y%4==0 and y%100!=0) else "Not Leap Year")
```

| Check     | Result |
| --------- | ------ |
| %400      | False  |
| %4 & %100 | True   |

**Result:** Leap Year
**Bro Explain:** Calendar rule pass

---

## 1️⃣2️⃣ Max of 3 Numbers (3,7,5)

```python
a,b,c = 3,7,5
print(max(a,b,c))
```

| Compare | Max |
| ------- | --- |
| 3 vs 7  | 7   |
| 7 vs 5  | 7   |

**Result:** 7
**Bro Explain:** Sabse bada choose

---

## 1️⃣3️⃣ Swap (Python) a=2,b=1

```python
a,b = 2,1
a,b = b,a
print(a,b)
```

| Step  | a | b |
| ----- | - | - |
| Start | 2 | 1 |
| Swap  | 1 | 2 |

**Bro Explain:** Python direct swap

---

## 1️⃣4️⃣ Swap (Math) a=5,b=3

```python
a,b = 5,3
a = a+b
b = a-b
a = a-b
print(a,b)
```

| Step  | a | b |
| ----- | - | - |
| a=a+b | 8 | 3 |
| b=a-b | 8 | 5 |
| a=a-b | 3 | 5 |

**Result:** Swapped
**Bro Explain:** Math trick

---

## 1️⃣5️⃣ Table Print (n=2)

```python
n = 2
for i in range(1,6):
    print(n*i, end=" ")
```

| i | n*i |
| - | --- |
| 1 | 2   |
| 2 | 4   |
| 3 | 6   |
| 4 | 8   |
| 5 | 10  |


| #  | Logic Name          | Pseudo Code   | Steps (Bro Language)                      | Overall Logic / Why Needed (Depth)                            | Iteration (Depth ≤5) | One-Line Python Main Logic                                        | Output (Example) |
| -- | ------------------- | ------------- | ----------------------------------------- | ------------------------------------------------------------- | -------------------- | ----------------------------------------------------------------- | ---------------- |
| 1  | Even / Odd          | n % 2 == 0    | Number lo → 2 se divide → remainder dekho | Modulus remainder batata hai number evenly divide hua ya nahi | Single check         | `print("Even" if n%2==0 else "Odd")`                              | n=4 → Even       |
| 2  | Positive / Negative | n > 0         | Number ko 0 se compare karo               | Zero reference se sign identify hota hai                      | Single condition     | `print("Positive" if n>0 else "Negative")`                        | n=-5 → Negative  |
| 3  | Prime               | loop 2 to n-1 | Har number se divide karke check          | 1 aur khud ke alawa koi factor mila → not prime               | i=2→3→4→5            | `print("Prime" if all(n%i for i in range(2,n)) else "Not Prime")` | n=7 → Prime      |
| 4  | Factorial           | fact*=i       | 1 se n tak multiply                       | Previous result next step ka base banta hai                   | 1→2→3→4→5            | `import math; print(math.factorial(n))`                           | n=5 → 120        |
| 5  | Fibonacci           | a+b=c         | Last 2 numbers add                        | Sequence previous 2 values pe depend hoti hai                 | 0,1→1→2→3            | `a,b=0,1; [print(a,end=" ") or (a:=b,b:=a+b) for _ in range(5)]`  | 0 1 1 2 3        |
| 6  | Reverse Number      | n%10          | Last digit nikalo                         | Mod se digit nikle, divide se digit remove                    | 123→12→1             | `print(int(str(n)[::-1]))`                                        | 123 → 321        |
| 7  | Palindrome          | rev == n      | Reverse + compare                         | Original aur reversed same ho to palindrome                   | Same as reverse      | `print("Yes" if s==s[::-1] else "No")`                            | aba → Yes        |
| 8  | Armstrong           | sum += d³     | Digit power sum                           | Digit ke cube ka sum original se match                        | d1→d2→d3             | `print("Yes" if sum(int(d)**3 for d in str(n))==n else "No")`     | 153 → Yes        |
| 9  | Sum of Digits       | sum+=n%10     | Digit add karo                            | Number tod ke digits ka sum                                   | Each digit           | `print(sum(map(int,str(n))))`                                     | 123 → 6          |
| 10 | Count Digits        | count++       | Digit count karo                          | Har divide ek digit remove karta hai                          | Each digit           | `print(len(str(n)))`                                              | 4567 → 4         |
| 11 | Leap Year           | %4,%100,%400  | Year rule check                           | Calendar rules combine hote hain                              | Single decision      | `print("Leap" if n%400==0 or (n%4==0 and n%100!=0) else "No")`    | 2024 → Leap      |
| 12 | Max of 3            | if a>b>c      | Compare values                            | Comparisons se largest select hota hai                        | 2–3 compares         | `print(max(a,b,c))`                                               | 3,7,5 → 7        |
| 13 | Swap (temp)         | t=a           | Extra variable use                        | Data loss avoid karne ke liye temp                            | 3 steps              | `a,b=b,a`                                                         | a=2,b=1          |
| 14 | Swap (no temp)      | a=a+b         | Math trick                                | Arithmetic se bina extra memory swap                          | 3 ops                | `a=a+b; b=a-b; a=a-b`                                             | swapped          |
| 15 | Table Print         | i*n           | Loop print                                | Loop se repetitive output                                     | 1→2→3→4→5            | `for i in range(1,6): print(n*i)`                                 | n=2 → 2 4 6 8 10 |
