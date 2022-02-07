# Multiple Sum

Given a positive number x, find the sum of all the multiples of 3 or 5 that are less than or equals to x. 
For example, if x = 12 then the multiples of 3 or 5 that are less than or equals to 12 
are 3, 5, 6, 9, 10, 12. The sum of these multiples is 45.

## Input Format:
First line contains T that denotes the number of test cases. This is followed by T lines, each containing an integer, x.

## Output format
For each test case, print an integer in a new line that denotes the sum of all the multiples of 3 or 5 <= x. 

## Constraints:
1 <= T <= 10^5
1 <= x <= 10^9

## Sample Input
2
12
15

## Sample Output
45
60

``` java
import java.util.Scanner;
class Result {
    static long multipleSum(int x) {
      // Write your code here
        long sum = 0;
        for (int i = 1; i <= x; i++) {
          if (i % 3 == 0 || i % 5 == 0)
            sum += i;
        }
        return sum;
    }
}

class Main {
  public static void main(String[] args)
  {
    int t;
    Result o1 = new Result();
    Scanner sc = new Scanner(System.in);
    t = Integer.parseInt(sc.nextLine().trim());
    while (t>0)
    {
      t--;
      int n = sc.nextInt();
      System.out.println(o1.multipleSum(n));
    }
  }
}

```
