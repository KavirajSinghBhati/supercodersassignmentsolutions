# Partition a Array

Given a randomly ordered array (arr) of n elements, function partitionArray(int arr[], int n, int x) 
partition the elements into two subsets such that elements <= x are in left subset and elements > x are in the right subset.

Initial code of partitionArray(int arr[], int n, int x) which is given fails in some test cases. 
Identify those test cases and make the necessary changes in the function so that it gives the desired output in all the cases.

## Input

First line of test case will contain two number n (number of elements in list ) and x (number to use for partition) separated by space. 
Next line will contain N space separated integers.

## Output

Print the array after partition one element in each line.

## Constraints

1 <= n <= 10^5
-(10^9) <= x, arr[i] <= 10^9

``` java
class Result {
  static void partitionArray(int arr[], int x)
  {
    int i, j, temp;
    int n = arr.length;
    i = 0;
    j = n-1;

    while (i < j)
    {
      while (arr[i] <=x)
        i++;
      while (arr[j] > x)
        j--;

      temp = arr[i];
      arr[i] = arr[j];
      arr[j] = temp;
    }
    temp = arr[i];
    arr[i] = arr[j];
    arr[j] = temp;
    i++;
    j--;
  }
}
```
