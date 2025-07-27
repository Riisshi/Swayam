```text
# MCQs on gcd Algorithm and Python Setup (NPTEL Week 1 Lectures 1-4)

1. **What does gcd(m, n) represent?**  
   A) The sum of m and n  
   B) The smallest number dividing both m and n  
   **C) The largest number dividing both m and n**  
   D) The difference between m and n  

2. **Which of the following is always a divisor of any integer?**  
   A) 0  
   **B) 1**  
   C) 2  
   D) The integer itself  

3. **What is the main drawback of the naive algorithm for computing gcd by listing all factors?**  
   A) It uses too much memory  
   B) It only works for prime numbers  
   **C) It is inefficient and takes too many steps for large numbers**  
   D) It cannot find any common factors  

4. **Which Python construct is appropriate when the number of repetitions is unknown upfront?**  
   A) for loop  
   B) if statement  
   **C) while loop**  
   D) try-except  

5. **In Euclid’s algorithm for gcd, what is the key mathematical property used?**  
   **A) If d divides both m and n, then d divides m-n**  
   B) gcd(m,n) = m + n  
   C) gcd(m,n) is always equal to 1  
   D) gcd(m,n) = max(m,n)  

6. **What is the output of gcd(18, 25) using Euclid's algorithm?**  
   A) 18  
   B) 25  
   **C) 1**  
   D) 43  

7. **In the recursive Python function for gcd using Euclid’s algorithm, what is the base case?**  
   A) when m equals n  
   B) when m < n  
   C) when m % n == 0  
   **D) when n == 0** *(Note: In the provided code, base case is when remainder is 0; equivalent to n == 0 in a variant)*  

8. **What does the expression m % n represent in Python?**  
   A) The quotient of m divided by n  
   B) The product of m and n  
   **C) The remainder when m is divided by n**  
   D) The sum of m and n  

9. **Why is Euclid’s algorithm considered efficient compared to the naive approach?**  
   A) It uses lists to store factors  
   B) It requires knowledge of prime factorization  
   **C) It reduces the problem size quickly by using remainders**  
   D) It uses multiplication instead of division  

10. **Which Python version is recommended for new learners as per the NPTEL material?**  
    A) Python 2.7  
    **B) Python 3+**  
    C) Python 1.5  
    D) JavaScript  

11. **What is the role of the Python interpreter?**  
    A) To compile programs into machine code  
    **B) To execute Python code directly, line by line**  
    C) To translate Python code into Java  
    D) To convert Python code into C++  

12. **Which of the following is NOT a platform where Python can be installed?**  
    A) Linux  
    B) MacOS  
    C) Windows  
    **D) None of the above**  

13. **How can you import all functions from a Python file named `filename.py` into an interpreter session?**  
    A) import filename.py  
    **B) from filename import ***  
    C) load filename  
    D) exec filename  

14. **Which statement about Python 2.7 vs 3.x is true?**  
    **A) Python 3.x removed some features to improve language consistency**  
    B) Python 3.x is identical to Python 2.7  
    C) Python 2.7 is for mobile only  
    D) Python 3.x cannot be installed on MacOS  

15. **What is the most recent common factor (mrcf) in the context of gcd algorithms?**  
    A) The smallest common factor found so far  
    **B) The most recent common factor found, potentially the largest so far**  
    C) The count of common factors found so far  
    D) The product of common factors  

16. **In the while loop implementation of gcd, what causes the loop to terminate?**  
    A) When m equals n  
    **B) When m % n is zero**  
    C) When n is less than m  
    D) When a new common factor is found  

17. **Which of the following is a good resource to learn Python programming?**  
    A) http://www.randomsite.com  
    **B) http://www.diveintopython3.net**  
    C) http://www.fakeurl.org  
    D) None of the above  

18. **What is a key reason to practice programming by writing and executing code?**  
    A) To memorize syntax rules only  
    **B) To appreciate how programming works in practice**  
    C) To avoid reading programming books  
    D) To run programs without errors  

19. **In the backward scan gcd algorithm, why do we start scanning from min(m,n) downward?**  
    **A) Because the gcd cannot be larger than min(m,n)**  
    B) To find the smallest factor first  
    C) To optimize memory usage  
    D) To avoid using loops  

20. **What happens in Euclid’s algorithm if n divides m exactly?**  
    A) The gcd is zero  
    B) The gcd is m  
    **C) The gcd is n**  
    D) The algorithm continues indefinitely  

21. **What does the division step m = qn + r represent in Euclid's algorithm?**  
    A) m is the sum of q, n, and r  
    **B) m divided by n gives quotient q and remainder r**  
    C) m multiplied by n equals q plus r  
    D) None of the above  

```