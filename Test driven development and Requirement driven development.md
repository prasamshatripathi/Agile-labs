##Test Driven Development(TDD) and Requirement Driven Development

OBJECTIVES:
->Understand and implement Test-Driven Development (TDD).

->Understand and implement Requirement-Driven Development (RDD).

->Compare TDD vs RDD approaches.

->Develop a small application module using both methods.

INTRODUCTION:

 TDD is a software development technique where tests are written before writing actual code.It follows the loop:
   1.Write a test.
   2.Run the test.
   3.Write a minimum code to pass the test.
   4.Refactor code.
   5.Repeat.

  RDD is a user-centric approach where development is directly driven by requirements (e.g., user stories, use cases). Here, developers write features directly based on the requirement, and testing is done after the implementation.

TOOLS AND TECHNOLOGY USED:

Language: Python 3
Testing Tool: unittest (for TDD)
Editor: VS Code / Jupyter / Colab

TEST-DRIVEN DEVELOPMENT:
PROBLEM STATEMENT:
         Create a function to check whether a number is prime using TDD.

         Step 1: Write a first test
            
  import unittest
from prime import is_prime  # This file doesn't exist yet

class TestPrime(unittest.TestCase):
    def test_prime(self):
        self.assertTrue(is_prime(7))
        self.assertTrue(is_prime(2))
        self.assertFalse(is_prime(4))
        self.assertFalse(is_prime(0))
        self.assertFalse(is_prime(1))

if __name__ == '__main__':
    unittest.main()

   step 2: Run the test (will fail because is_prime doesn't exist)

 Step 3: Create actual implementation
     
       def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, int(n**0.5)+1):
        if n % i == 0:
            return False
    return True


Step 4: Run the test.

Step 5: REfactor if needed.

  
  REQUIREMENT -DEIVEN DEVELOPMENT
Requirement:
Develop a calculator function that adds and multiplies numbers based on user stories.

User Stories:
As a user, I want to add two numbers.
As a user, I want to multiply two numbers.

code:
class Calculator:
    def add(self, a, b):
        return a + b

    def multiply(self, a, b):
        return a * b


calc = Calculator()
print("Add:", calc.add(5, 3))         # Output: 8
print("Multiply:", calc.multiply(5, 3))  # Output: 15


CONCLUSION:

 ->TDD ensures high code reliability and fewer bugs.
->RDD aligns development with end-user needs and focuses on feature delivery.
->Combining both gives the best of both worlds in Agile.

