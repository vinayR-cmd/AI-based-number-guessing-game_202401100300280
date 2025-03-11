The Core Idea
The goal of this project is to create an AI-powered number guessing game where the AI efficiently guesses a secret number chosen by the user. Instead of randomly guessing, the AI should minimize the number of attempts required to find the correct number using a logical approach.

Understanding the Problem
Imagine a scenario where you have a number in mind between 1 and 100, and an AI is trying to guess it. The AI should:

Make a guess.
Receive feedback (whether the guess is too high, too low, or correct).
Use this feedback to refine its future guesses.
Continue until the correct number is found.
A naïve approach would be for the AI to randomly pick numbers. However, this is inefficient because it may take up to 100 attempts in the worst case.

The Challenge
The AI needs to find the correct number in the shortest number of guesses possible.
The AI should eliminate incorrect numbers quickly based on feedback.
The AI must handle user inputs efficiently and provide meaningful feedback like:
"Too high" (the guessed number is greater than the secret number).
"Too low" (the guessed number is smaller than the secret number).
"Correct!" (the AI found the number).
Real-World Analogy
This problem is similar to how a search algorithm works in real-world applications.
For example:

A binary search algorithm used in databases to find records efficiently.
AI-powered search engines that narrow down results based on user input.
An AI assistant that guesses user preferences based on past interactions.
The Optimal Solution: Using Binary Search
To solve this problem efficiently, we implement a binary search strategy, which:

Starts with a middle number (e.g., 50 in a range of 1-100).
If the guess is too high, the AI eliminates all numbers greater than the guess.
If the guess is too low, the AI eliminates all numbers smaller than the guess.
The AI keeps narrowing down the range until it finds the correct number.
This approach ensures the AI always finds the correct number within at most 7 guesses (since log₂(100) ≈ 7).

Conclusion
The problem requires an efficient, intelligent approach to guessing numbers. Using binary search, the AI can find the correct number much faster than random guessing, demonstrating the power of algorithmic thinking in AI applications. 🚀
