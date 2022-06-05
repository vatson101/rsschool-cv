# Sergey Gumba
## Contacts
* **Location:** T'bilisi, Georgia
* **Phone:** *+995 551 589 721*
* **Email:** prokrion@gmail.com
* **Telegram** @vatson101

## About me 
I've been attracted to IT and programming since a rather young age. In my high school days I started learning **Java** and tried to make a platformer game. Though I haven't completed the game, through this experience I've learned a lot of various useful skills: from **OOP**, image managing, collisions problem and ending with general problem-solving abilities. 

Despite my current profession being quite far from IT, throughout the following years programming has been my interest and a hobby. Currently I'm using **Pyton 3** for my projects. The most recent of these projects is building a very basic neural network that can recognize handwritten digits. As I was studying for 2 and half years in a technical univercity, I managed to use Calculus and Algebra to code the backwards propagation algorithm.

As for my soft-skills, I'm very comunicative, enthusiastic, I really like learning new things and to use them practically to achieve better results. 

## Skills
* Java and Python 3
* OOP, Algorithms
* Calculus, Algebra
* VS Code
* Git and GitHub

## Code Example
"Subarray sum equals k" from leetcode.com: Given an array of integers nums and an integer **k**, *return the total number of subarrays whose sum equals to* **k**.

A subarray is a contiguous **non-empty** sequence of elements within an array.

```from collections import defaultdict

arr0 = list(input().split(' '))
arr = [int(x) for x in arr0]
k = int(input())

dict = defaultdict(lambda: 0)
dict[0] = 1
subsum = 0
counter = 0
for i in range(len(arr)):
    subsum += arr[i]
    if subsum - k in dict:
        counter += dict[subsum - k]
    dict[subsum] += 1
    
print(counter)```