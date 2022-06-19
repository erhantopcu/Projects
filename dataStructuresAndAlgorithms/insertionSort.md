[Profile](https://app.patika.dev/erhntopcu)

### [22,27,16,2,18,6] -> Insertion Sort

1. Write the stages of the above sequence according to the sort type.
2. Write the Big-O notation.
3. Time Complexity: Average case: The number we are looking for is in the middle, Worst case: The number we are looking for is at the end, Best case: The number we are looking for is at the beginning of the series.
4. What case does the number 18 fall into after the array is sorted?
5. Write the first 4 steps of [7,3,5,8,2,9,4,15,6] according to Insertion Sort.

## Answers
# 1.
**[[22],27,16,2,18,6]**
Note: The part separated by '[' and ']' brackets represents the currently sorted range.

***Step1.***
> newList : [16,22],27,2,18,6

***Step2.***
> newList : [16,22,27],2,18,6

***Step3.***
> newList : [2,16,22,27],18,6

***Step4.***
> newList : [2,16,18,22,27],6

***Step5.***
> newList : [2,6,16,18,22,27]

# 2.
Average case : When we take the average of the worst case and the best case, we find it as n^2.
> O(n^2)

# 3.
Worst case : PERFECT INVERSION, in which case each element of the array will be less than the one behind it. So for the 1st element, the inner loop will move 0 backwards 1 for 2 elements, two for the 3rd element, then back 3 4 5 6… n. So 0+1+2+3+4…..+n-1 = [n*(n-1)]/2 : n^2
Best case : FULL SEQUENCE goes over n numbers once and stays with this one pass as there is no need to advance any of them backwards. So n
Average case : When we take the average of the worst case and the best case, we find it as n^2.

# 4.
After the array is sorted, since the number 18 is in the middle of the array; It falls under the "Average Case".

# 5.
 [7,3,5,8,2,9,4,15,6]

***Step1.***
[3,7],5,8,2,9,4,15,6

***Step2.***
[3,5,7],8,2,9,4,15,6

***Step3.***
[3,5,7,8],2,9,4,15,6

***Step4.***
[2,3,5,7,8],9,4,15,6