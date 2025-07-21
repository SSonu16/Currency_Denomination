# Currency_Denomination
Currency Denomination using Greedy strategy (ATM)


 Problem Statement
When a person withdraws cash from an ATM, the machine must dispense the exact amount using available denominations like ₹2000, ₹500, ₹200, ₹100, ₹50, etc.
The goal is:
•	To minimize the number of currency notes dispensed.
•	To ensure accuracy (the total must exactly match the withdrawal amount).



The greedy algorithm solves this by:
1.	Always choosing the largest denomination first that does not exceed the remaining amount.
2.	Subtracting that value from the amount.
3.	Repeating the process until the remaining amount is zero.
This strategy doesn’t reconsider choices — it takes what seems best at each step, trusting that this leads to an optimal overall solution.
For currencies like the Indian Rupee, where denominations are multiples or near-multiples of smaller ones (e.g., 500 is a multiple of 100, 100 is a multiple of 50), the greedy approach is guaranteed to produce the optimal solution (least number of notes).
Example:
Amount = ₹3850
Denominations = [2000, 500, 200, 100, 50, 20, 10, 5, 2, 1]
Greedy picks: 1 x 2000, 3 x 500, 1 x 200, 1 x 100, 1 x 50 → total = ₹3850 using only 7 notes.



Objectives 
•	To implement a greedy strategy for solving the currency denomination problem.
•	To minimize the number of notes dispensed for a given withdrawal.
•	To improve the efficiency of cash dispensing in ATMs.
•	To analyse and evaluate the algorithm’s performance and time complexity.
•	To test the solution for various inputs to ensure reliability.


Time and Space Complexity

•	Time Complexity:
o	Sorting: O(n log n) (once, for denominations).
o	Main loop: O(n) for n denominations.
o	Overall Time Complexity: O(n log n) , but effectively constant for fixed denominations (e.g., 10 values).
o	The algorithm runs in O(n) time, where n is the number of available denominations.
Since the number of denominations in a real-world scenario (like Indian currency) is constant, the time complexity is effectively O(1).

•	Space Complexity:
o	The space required to store the result is O(n) (one count per denomination).


  Result

Enter the amount to withdraw: ₹3897
Denomination Breakdown:
₹2000 x 1
₹500 x 3
₹200 x 1
₹100 x 1
₹50 x 1
₹20 x 2
₹5 x 1
₹2 x 1 



