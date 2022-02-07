# Cut the chocolate smartly for maximum pieces

Mr. G wants to impress his sister by giving her a lot of chocolate pieces. Assume he has a giant rectangular chocolate bar. 
Now your task is to find the maximum number of chocolate pieces, that he can cut and give to his sister, 
keeping in mind the below given conditions

    The chocolate must be served as only 1 x 1 sized pieces
    He can cut the chocolate bar exactly K times.


Complete the maxPieces() function in editor. 
It has 1 parameter i.e. an integer denoting the value of K, 
and it must return an integer denoting the maximum number of chocolate pieces that can be cut.

## Input Format

The first line contains an integer T, denoting the number of test cases. 
Each of Next T lines contains an integer K.

## Output Format

For each test case, return the maximum number of pieces(1 x 1 sized) that can be cut, given the value of K.

## Constraints

1 <= T <= 100
0 <= K <= 10^9

## Sample Input

3
7
5
6

## Sample Output

12
6
9

```java
import java.io.*;
import java.math.*;
import java.util.*;

class Result {
  static long maxPieces(int k) {
    // Write your code here
    long maxPieces = 0;
    int horizontalCuts = k / 2;
    int verticalCuts = k - horizontalCuts;
    maxPieces = horizontalCuts * verticalCuts;
    return maxPieces;
  }
}

class Main {
  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    int t = Integer.parseInt(sc.nextLine().trim());
    while(t > 0)
    {
      int k = sc.nextInt();
      System.out.println(Result.maxPieces(k));
      t--;
    }
  }
}

``` 
