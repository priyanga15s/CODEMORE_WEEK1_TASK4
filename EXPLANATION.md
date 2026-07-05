# Explanation of Java Concepts Used

## Objective

This program performs three operations on an integer array:

1. Finds the largest element.
2. Finds the smallest element.
3. Reverses the array.

---

# 1. Scanner Class

The `Scanner` class is used to receive input from the user.

```java
Scanner sc = new Scanner(System.in);
```

Methods used:

- `nextInt()` – Reads integer values.

---

# 2. Array Declaration

An integer array is created using the size entered by the user.

```java
int[] arr = new int[n];
```

Example:

If the size is 5, the array stores five integer values.

---

# 3. Input Using a Loop

A `for` loop stores the array elements.

```java
for(int i = 0; i < n; i++) {
    arr[i] = sc.nextInt();
}
```

Each element is stored using its index.

---

# 4. Finding the Largest and Smallest Elements

Initially, the first element is assumed to be both the largest and the smallest.

```java
int largest = arr[0];
int smallest = arr[0];
```

The program then compares each remaining element.

Largest:

```java
if(arr[i] > largest)
```

Smallest:

```java
if(arr[i] < smallest)
```

---

# 5. Reverse Array Function

A separate method is created to reverse the array.

```java
public static void reverseArray(int[] arr)
```

Two variables are used:

- `start` points to the beginning.
- `end` points to the last element.

Elements are swapped until both pointers meet.

```java
int temp = arr[start];
arr[start] = arr[end];
arr[end] = temp;
```

Then:

```java
start++;
end--;
```

This efficiently reverses the array.

---

# 6. Displaying the Reversed Array

A `for` loop prints each element.

```java
for(int i = 0; i < n; i++)
```

---

# 7. Closing the Scanner

```java
sc.close();
```

This releases system resources.

---

# Program Flow

1. Read the size of the array.
2. Read all array elements.
3. Assume the first element is both the largest and smallest.
4. Traverse the array to find the actual largest and smallest elements.
5. Call the `reverseArray()` method to reverse the array.
6. Display the reversed array.
7. Close the Scanner.
8. End the program.

---

# Java Concepts Covered

- Scanner Class
- Arrays
- Array Indexing
- Variables
- For Loop
- While Loop
- If Statements
- Methods (Functions)
- Swapping Technique
- Array Traversal
- Output Statements
- Resource Management (`sc.close()`)
