Explanation of the Code
​This C program reverses the digits of an integer provided by the user. The core logic relies on a while loop and basic arithmetic operations.
​Key Logic & Steps:
​Variable Initialization: * n: Stores the input number.
​rev: Stores the reversed result (initialized to 0).
​rem: Stores the remainder (the last digit of the current number).
​The While Loop (while (n != 0)):
The loop continues as long as n is not zero. Inside the loop, three main steps happen:
​Extracting the last digit: rem = n % 10;
This uses the modulus operator to get the last digit of the number. For example, if n is 123, 123 % 10 gives 3.
​Building the reversed number: rev = (rev * 10) + rem;
Here, we multiply the current rev value by 10 to shift its digits to the left and then add the extracted digit (rem). This effectively builds the number in reverse order.
​Updating the number: n = n / 10;
We divide n by 10 to remove the last digit that was just processed. Since n is an integer, this division discards the decimal part.
​Completion:
The loop terminates when n becomes 0, and the final reversed value is stored in rev, which is then printed to the console.
