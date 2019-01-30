## Paper Review X

- Reviewer: Sang Oh
- Paper Title: Hash-based carving: Searching media for complete files and file fragments with sector hashing and hashdb
- Author: Simson L. Garfinkel, Michael McCarin 

### Did you like this paper?  Why?
- 1-2 sentences
Yes, the graphics explaining what overlapping 4kb sectors on page 5 greatly helped me to understand the purpose of needing to test all possible alignments to account for different file system offsets. The paper was also very thorough in explaining all aspects of the new method so that areas of improvement and areas lacking could easily be distinguished by readers.

### What problem is this paper solving?
- 2-3 sentences
This paper is solving the problem of making a feasible method of hash-based carving that is efficient and accurate. This was accomplished by using a preassembled hash database used in conjunction with the HASH-SETS algorithm, which identifies disk sectors of interest, and the HASH-RUNS algorithm, which actually reassembles the files.

### What are the strengths of this paper?
- 3-4 sentences
The strengths of this paper are that it contains adequate breadth and depth of the topic at hand. It also references and builds upon prior work in this field so that readers can grasp the context and progress in feasible hash-based carving. The authors are also not shy about sharing the details of their failures, which will help future innovators to avoid the same mistakes.

### What are the main weaknesses in the paper?
- 3-4  sentences
The main weakness of this paper is the lack of clear simple explanation for the purpose of hash-based carving for people that be unfamiliar with hashes or even digital forensics. There is also a lack of explanation of what whole-file hashing and why it's less optimal than hash-based carving. Lastly, the tests are run on a computer with 64 cores, which doesn't help to put into perspective how applicable this may be on personal computers. At least an estimate of how long it would
take to run on commercial personal computers could've offered a good point of comparison for base users.

### Next Steps?
- What  would  you do differently?
- Are there assumptions you disagree with?
- Do you see ideas for future work or improving the solution?
- Do you see new attack vectors/vulnerabilities?    
    - 5-6 sentences
I would add in a usability section where people unfamiliar with this project are given the tools and asked to work on a simple example of extracting a file. Tools can be complex and efficient, but they are of no use in the big picture if only a couple people, like the people who developed them, can use it. There must be adequate work put into making tools usable by the lowest skill level possible. I would have also appreciated a breakdown on the accuracy of the algorithms with respect
to different file types. It seemed like the authors had more success with text files than video or similarly more complex file types. I do not see a clear direction for future work except for improving the efficiency and accuracy of the algorithm to a minor extent. An easy defense from this method would be to encrypt your hard drive.


## How to Read a Paper

### 1. Category
    - What type of paper is this?
    - A measurement paper?  An analysis of an existing system? A description of a research prototype?
    This paper is a demonstration of the improvement of hash-based carving and its feasibility stemming from its efficiency and accuracy.

### 2. Context
    - Which other papers is it related to?
    - Which theoretical bases were used to analyze the problem?
Much of the paper is related to prior work by Garfinkel, one of the authors, on developing methods for hash-based carving. The paper describes a feasible way to use hash-based carving in practice by solving the problem of certain issues that negatively affected either accuracy or efficiency. The paper does not delve too deeply into proving on why the new method is algorithmically sound.

### 3. Correctness
    - Do the assumptions appear to be valid?
A big assumption of the practicality of this method is that the disk is unencrypted. It may be in the close future that any disk drives worth investigating are encrypted by criminals to prevent incriminating evidence to be discoverable using this method.

### 4. Contributions
    - What are the paper’s main contributions?
The paper contributed a feasible means of hash-based carving with 2 new algorithms. It also suggested avenues of improvement for future use because current performance on a 13 gb drive is good but slow.

### 5. Clarity
    - Is the paper well written?
The paper is fairly well written, especially with the abundant use of subheadings to separate ideas and clearly step through parts of the experiments. There is a great level of detail which makes it easy for people to extend upon this topic with their own experiments and innovations.
