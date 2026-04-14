# JS-Assignment

This is my submission for Assignment 4 Fundamentals of Web Design.

Question 1: Digit Gatekeeper
*Approach:* I used a basic `for` loop to go from `L` to `R-1`. First, I check if the number is divisible by `K`. If it is, I convert it to a string to check each digit. I count if there are any '0's. If there are no zeros, I add all the digits to get the sum. To check if the sum is prime, I count its factors using another loop. If factors are exactly 2, I increase my main answer count.
*Complexity:*
- *Time Complexity:* O(N * D) where N is the difference between L and R, and D is the number of digits.
- *Space Complexity:* O(1) because I am only storing a few simple variables.

Question 2: Roll-Seed Lock
*Approach:* I started with the input number `N` and ran a `for` loop exactly 3 times. Inside the loop, I used an `if-else` condition to check if the number is even or odd, and did the math given in the question. Finally, I checked if the result is between 100 and 999. To match the middle digit with the seed, I converted the number to a string and checked the character at index 1.
*Complexity:*
- *Time Complexity:* O(1) because the loop always runs exactly 3 times.
- *Space Complexity:* O(1) 

Question 3: Mirror Corridor
*Approach:* I needed to find the smallest number `X` to add to `N`. So, I ran a loop for `X` from 0 to 10000. For every number, I checked if `(N + X)` is divisible by `K`. If yes, I converted the number to a string and manually reversed it using a backwards `for` loop. If the original string and the reversed string were the same, it means it's a palindrome number, so I saved that `X` and stopped the loop using `break`.
*Complexity:*
- *Time Complexity:* O(1) in the worst case because the limit is fixed at 10000.
- *Space Complexity:* O(1)

Question 4: Fare Calculator
*Approach:* I solved this step-by-step just like the rules were given. First, I calculated the basic fare. Then I used `if` conditions to add extra charges for late minutes and distance. For the seed rule, I checked if `seed % 2 == 1` (odd) to subtract it, otherwise added it. Finally, to round up to the nearest multiple of 5, I found the remainder (`fare % 5`) and added the difference instead of using complicated math functions.
*Complexity:*
- *Time Complexity:* O(1) because it's just simple math and no loops are used.
- *Space Complexity:* O(1)

Question 5: Skipping Numbers
*Approach:* I used a `while` loop that keeps running as long as my `sum` is less than `N`. I created a variable `m` starting from 0 and increased it by 1 every time. Then I checked if `m` is NOT divisible by `(seed + 2)`. If it is not divisible, I added it to my sum. The loop stops automatically when the sum reaches or crosses `N`.
*Complexity:*
- *Time Complexity:* O(M) where M is the final number we reach. 
- *Space Complexity:* O(1)

 Question 6: Contest Score Judge
*Approach:* I first calculated the raw score using the formula `3*a + b - 2*c`. Then I just used simple `if` statements. If the score was below 0, I changed it to 0. If the total answers `(a + b + c)` were more than 50, I reduced the score by 10. At the very end, an `if-else` block checks if the final score is 60 or more to print PASS, else FAIL.
*Complexity:*
- *Time Complexity:* O(1) because there are no loops, just basic calculations.
- *Space Complexity:* O(1)
