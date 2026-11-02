How to calculate Time Complexity?
Remember these rules:
Java code pattern	Complexity
Single statement	O(1)
One loop	O(n)
Two nested loops	O(n²)
Three nested loops	O(n³)
Loop dividing by 2	O(log n)
Two separate loops	O(n + n) = O(n)
Nested loop plus single loop	O(n² + n) = O(n²)

Rule: Ignore constants and lower-order terms.

For example:
\[
O(3n^2+5n+10)=O(n^2)
\]
