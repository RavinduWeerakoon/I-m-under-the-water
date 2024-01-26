## Help me pls 
This is a question which I have added for the mora extreme 8.0 which is the sri lankas largest algorithmic coding compition organized by the IEE CS branc of university of Moratuwa. The problam is at the medium level with 8% solvable eat
Feel free to try the question and this is the description

A person is locked inside a cage underwater, screaming "I'm under the water! Please Help me".And the cage can’t be broken mechanically as some unknown transparent strong material made it. But a programmer can free him ��. 

To release him, you need to find a way to build the codeword. However, after you break the codeword, there is some time that it will take to open the cage. This time is calculated according to the following rules:
 - At first, you are given an empty string. 
 - There are two restrictions: 
 - The codeword must have a length of l. 
 - When you add a character to the string, the time is increased by "p" seconds. 
 - When you duplicate the string, the time is increased by level "q" seconds. 

Find the minimum amount of time to open the cage so that the person underwater can stop screaming.


A person is locked inside a cage underwater, screaming "I'm under the water! Please
Help me".And the cage can’t be broken mechanically as some unknown transparent
strong material made it. But a programmer can free him 😎.

[Little message from him](https://youtu.be/S8qbu7ZcTYM?si=jr3qJkJUFwn-8v2n)

To release him, you need to find a way to build the codeword. However, after you break the codeword, there is some time that it will take to open the cage. This time is calculated according to the following rules:


- At first, you are given an empty string. 
- There are two restrictions: 

1. The codeword must have a length of L. 
2. When you add a character to the string, the time is increased by "p" seconds. 
3.Copy any substring from the code that you are bulding and add it to the end. This will increase the time by q second .
Ex : - codeword aabaacaba
          Lets think that you have built the code upto ‘aab’
You can create  ‘aabaa’ by only increasing q seconds as the ‘aa’ substring is in “aab”

Find the minimum amount of time to open the cage so that the person underwater can stop screaming.

Input Format

The first line $T$ contains number of testcases .
The $2 * T$ subsequent lines each describe a test case over lines:
The first contains $3$ space-separated integers $l$, $P$and $Q$ respectively.
The second contains Codeword $S$

Constraints
$1 <= T <=3$
$1 <= L <= 10^4$
$1 <= P,Q <= 1000$
$S$ is composed with lowercase letters only

Output Format
On a single line for each test case, print the minimum number of seconds which will be taken to open the door
Smaple Input
2 
9 4 5 
aabaacaba 
9 8 9 
bacbacacb  .
Smaple Output
26
42 
Explanation
Test case 0
Initial = “” ; final = “aabaacaba”
Append “a”; S = “a”; increases by 4 seconds
Append “a”; S = “aa”; increases by 4 seconds
Append “b”; S = “aab”; increases by 4 seconds
Copy and append “aa”; S=”aabaa” cost is 5;
Append “c”; S =”aabaac” cost is 4
Copy and Append “aba”; S=”aabaacaba” cost is 5

Summing each we get 4+4+4+5+4+5 = 26 output for the test case 1 is 26




