# Level 1 - CP Fundamentals

## 1. Complexity & Constraints
* **Input Handling for Competitive Programming**
  * Reading input correctly: single values, multiple values on one line, multiple test cases
  * Reading until EOF (`while(cin >> x)`)
* **Fast I/O**
  * `ios_base::sync_with_stdio(false); cin.tie(NULL);`
  * Why this matters once loops get large
* **Data type ranges**
  * `int` vs `long long` - overflow awareness
  * `float` vs `double` - precision issues, why CP avoids floating-point comparisons when possible
* **Type casting**
  * Implicit vs explicit casting
  * `(int)`, `(double)` conversions and common bugs from truncation
* **Brute force**
  * Writing the naive solution first before optimizing
  * Using brute force to generate test cases / verify faster solutions
* **Complexity intuition**
  * Big-O basics: $O(1)$, $O(\log n)$, $O(n)$, $O(n \log n)$, $O(n^2)$, $O(2^n)$
  * Counting nested loops and operations per element
* **Choosing an approach from constraints**
  * $n \le 10 \rightarrow$ exponential okay, $n \le 10^4 \rightarrow O(n^2)$ okay, $n \le 10^6 \rightarrow O(n \log n)$, $n \le 10^8 \rightarrow O(n)$

### Problems
* Predict output/complexity of given code snippets
* Handle multiple test cases ($t$ test cases per input file)
* Sum of large numbers requiring `long long`
* Fast I/O speed comparison on large input

---

## 2. Arrays & Traversal
* `vector` - declaration, `push_back`, resizing, indexing
* **Traversing** - index-based, range-based `for`
* **Sum, min, max** - running sum, `*max_element()`, `*min_element()`
* **Counting** - elements matching a condition
* **Searching** - linear search, existence check
* **Adjacent elements** - patterns comparing `a[i]` and `a[i+1]`, consecutive elements

### Problems
* Find max/min and their indices in an array
* Count elements greater than average
* Find second largest/smallest
* Check if array is sorted
* Move all zeros to the end
* Find the longest run of adjacent equal/increasing elements

---

## 3. Strings
* **Traversal** - character-by-character iteration
* **Character operations** - ASCII values, `isupper`/`islower`/`isdigit`, case conversion
* **Counting** - character frequency, vowel/consonant counts
* **Reversing** - `reverse()`, manual two-pointer reversal
* **Palindrome** - full string and substring checks
* **Transformations** - concatenation, `substr()`, case toggling

### Problems
* Check if a string is a palindrome
* Count vowels/consonants/digits in a string
* Reverse words in a sentence
* Check if two strings are anagrams
* Remove duplicate characters from a string

---

## 4. Basic Mathematics & Number Theory
* Even/odd, divisibility, modulo, integer division
* **Digits** - extraction, digit sum, digit count, reversing a number
* **Basic formulas** - sum of $n$ numbers, AP/GP basics, factorial
* **GCD & LCM** - Euclidean algorithm, `__gcd()`

### Problems
* Check if a number is prime (basic trial division)
* Sum of digits of a number
* Reverse a number and check palindrome
* Find GCD and LCM of two/more numbers
* Count divisors of a number

---

## 5. Frequency & Counting
* **Frequency arrays** - fixed-range counting
* **`map`** - ordered key-value counting
* **`set`** - uniqueness, membership testing
* **`unordered_map` basics** - $O(1)$ average lookup
* **`unordered_set` basics** - fast uniqueness checks
* **Distinct elements** - counting unique values
* **Duplicate detection** - using `set`/`map` to flag repeats

### Problems
* Find the most frequent element in an array
* Check if an array has any duplicates
* Find all distinct elements in a range
* First non-repeating character in a string
* Two arrays - check if they contain the same elements (regardless of order)

---

## 6. Sorting & Basic STL Algorithms
* `sort()` - default ascending, subranges
* `reverse()` - full/partial ranges
* **Sorting pair** - lexicographic ordering
* **Basic custom comparator** - lambda, sort by second value, descending order
* `min()`, `max()`, `swap()`
* `find()`, `count()`

### Problems
* Sort an array of pairs by second value
* Sort strings by length, then alphabetically (custom comparator)
* Find $k$-th smallest/largest element after sorting
* Merge two sorted arrays
* Count pairs with a given sum in a sorted array

---

## 7. Basic Bitwise Operations
* Binary representation
* AND (`&`), OR (`|`), XOR (`^`)
* Left shift (`<<`), right shift (`>>`)
* Check/set/unset/toggle bits
* Basic XOR properties

### Problems
* Check if a number is a power of 2
* Count set bits in a number
* Find the single non-repeating element (XOR trick)
* Swap two numbers using XOR
* Convert decimal to binary and back

---

## 8. Stack & Queue
* `stack`, `queue`, `priority_queue`
* LIFO vs FIFO
* **Basic operations:** `push`, `pop`, `top`, `front`, `back`, `empty`
* **Basic applications:**
  * Parentheses/bracket matching
  * Processing elements in order

### Problems
* Valid parentheses/bracket matching
* Next greater element (stack-based)
* Reverse a string/array using a stack
* Implement a queue using two stacks
* Simulate a simple task queue / Josephus-style problem

---

## 9. Basic Greedy
* Simple greedy choices
* Sorting + greedy
* Min/max optimization
* Basic greedy reasoning

### Problems
* Activity selection (max non-overlapping intervals)
* Minimum coins for a given amount (with given denominations)
* Fractional knapsack
* Assign cookies / minimize maximum difference problems

---

## 10. Prefix/Suffix Techniques
* Precomputation
* 1D prefix sum
* Range sum queries
* Suffix sum basics

### Problems
* Answer multiple range-sum queries efficiently
* Find equilibrium/pivot index of an array
* Maximum subarray sum of fixed length $k$ using prefix sums
* Difference array for range update problems

---

## 11. Basic Two Pointers
* Left/right pointers
* Same-direction pointers
* Pair problems
* Simple pointer-based optimization

### Problems
* Two-sum on a sorted array
* Remove duplicates from a sorted array in-place
* Container with most water
* Merge two sorted arrays using two pointers

---

## 12. Sliding Window
* Fixed-size window
* Variable-size window
* Expanding/shrinking window based on a condition

### Problems
* Maximum sum subarray of size $k$
* Longest substring without repeating characters
* Smallest subarray with $\text{sum} \ge \text{target}$
* Count subarrays with exactly $k$ distinct elements

---

## 13. Binary Search
* Binary search on arrays
* Binary search on answer
* Monotonic predicate reasoning

### Problems
* Find element in a sorted array (`lower_bound`/`upper_bound`)
* Find first/last occurrence of an element
* Binary search on answer: minimum capacity to ship packages in $D$ days
* Square root of a number using binary search

---

## 14. Basic Recursion
* Base cases
* Recursion tree intuition
* Simple backtracking

### Problems
* Factorial and Fibonacci using recursion
* Sum of digits / power of a number recursively
* Generate all subsets of a set
* Generate all permutations of a string