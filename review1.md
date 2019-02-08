## Paper Review 0

- Reviewer: Sang Oh
- Paper Title: An Analysis of China's "Great Cannon"
- Author: Bill Marczak; Nicholas Weaver; Jakub Dalek; Roya Ensafi

### Did you like this paper?  Why?
- Yes, the paper described all the information the researchers gained by using relatively simple tools.
They didn't use complicated techniques, rather, they took the data they were able to get and were able to logically conclude very important pieces of information about China's Great Cannon.
The paper also compares and contrasts the Great Cannon with the Great Firewall.

### What problem is this paper solving?
- This paper is solving the mystery of China's Great Cannon.
Not much is known about this private government tool, especially its capabilities and functions.
The authors are able to generally locate the system and describe its basic functions.

### What are the strengths of this paper?
- The strengths of this paper are that it divides up each piece of information up into short digestible sections.
There is good partitioning between topics, almost as if I didn't need to know about GreatFire.org's Logs to the history of the GC.
There is also a variety of articles cited where the authors are able to come to conclusions using pieces of information gleaned from events or incidents in combination with the results of their tests with the Chinese network.

### What are the main weaknesses in the paper?
- The main weakness of this paper is the lack of clear simple explanation for the purpose of hash-based carving for people that be unfamiliar with hashes or even digital forensics.
There is also a lack of explanation of what whole-file hashing and why it's less optimal than hash-based carving.
Lastly, the tests are run on a computer with 64 cores, which doesn't help to put into perspective how applicable this may be on personal computers.
At least an estimate of how long it would take to run on commercial personal computers could've offered a good point of comparison for base users.

### Next Steps?
- I would add in a usability section where people unfamiliar with this project are given the tools and asked to work on a simple example of extracting a file.
Tools can be complex and efficient, but they are of no use in the big picture if only a couple people, like the people who developed them, can use it.
There must be adequate work put into making tools usable by the lowest skill level possible. I would have also appreciated a breakdown on the accuracy of the algorithms with respect to different file types.
It seemed like the authors had more success with text files than video or similarly more complex file types.
I do not see a clear direction for future work except for improving the efficiency and accuracy of the algorithm to a minor extent.
An easy defense from this method would be to encrypt your hard drive.


## How to Read a Paper

### 1. Category
- This paper is a demonstration of the improvement of hash-based carving and its feasibility stemming from its efficiency and accuracy.

### 2. Context
- Much of the paper is related to prior work by Garfinkel, one of the authors, on developing methods for hash-based carving.
The paper describes a feasible way to use hash-based carving in practice by solving the problem of certain issues that negatively affected either accuracy or efficiency.
The paper does not delve too deeply into proving on why the new method is algorithmically sound.

### 3. Correctness
- A big assumption of the practicality of this method is that the disk is unencrypted.
It may be in the close future that any disk drives worth investigating are encrypted by criminals to prevent incriminating evidence to be discoverable using this method.

### 4. Contributions
- The paper contributed a feasible means of hash-based carving with 2 new algorithms.
It also suggested avenues of improvement for future use because current performance on a 13 gb drive is good but slow.

### 5. Clarity
- The paper is fairly well written, especially with the abundant use of subheadings to separate ideas and clearly step through parts of the experiments.
There is a great level of detail which makes it easy for people to extend upon this topic with their own experiments and innovations.
