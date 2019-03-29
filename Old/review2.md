## Paper Review 2

- Reviewer: Sang Oh
- Paper Title: Robust Signatures for Kernel Data Structures
- Author: Brendan Dolan-Gavitt; Abhinav Srivastava; Patrick Traynor; Jonathon Giffin

### Did you like this paper?  Why?
Yes, this method is dynamic and could be extended to other data structures and possibly other OS's.
Although there is a lot of setup involved with pinpointing robust kernel data structures, the process is well documented.
There is even a pseudo-code snippet describing part of the process.
Seeing exactly how features were being used in python helped to grasp what work was being done in the kernel.
This outputs a plugin for Volatility, which applies to what we directly learned in lab.

### What problem is this paper solving?
This paper proposes a solution to detecting objects hidden by kernel-mode rootkits.
Other tools use signatures from kernel data structures that are not reliable because the fields can be modified.
This new tool dynamically creates signatures for kernel data structures that are able to create signatures that can find more hidden objects.

### What are the strengths of this paper?
The paper used a Windows VM to test the process.
Windows is widely used so this demonstrated the practical use of this tool.
The paper clearly identifies assumptions before any predictions or results are put forth.
There was adequate discussion on issues with robust feature detection and any inefficiencies were well justified or accounted for with workarounds.

### What are the main weaknesses in the paper?
Parts of the paper are a bit repetitive.
It repeats information and concepts like in 4. Architecture and 4.1 Data Structure Profiling.
Quantitatively, this method yielded only a small improvement in performance from psscan2 and PTFinder

### Next Steps?
Further work should be done to streamline and speed up the process of coming up with signatures from robust features.
The process should be generalized to other data structures on Windows and even Linux.
More trials should be done with fuzzing for longer time periods to get better features.

## How to Read a Paper

### 1. Category
This paper proposes a novel method of detecting objects hidden by rootkits.

### 2. Context
Virus detection has easily been thwarted by metamorphic viruses which have significantly increased the difficulty of discovery.
However, the syntax of kernel data structures is controlled by the code of the OS.
Generating signatures based on these data structures is more robust because they cannot be changed by the attacker.
Pieces of this tool have been used in similar fashion by other tools.
Dynamic analysis of profile field usage in bbcache.
Fuzzing in Solar Eclipse.
Data structure invariants in Gibraltar.

### 3. Correctness
I was convinced by the way features were chosen based on profiling and fuzzing.
The logic was sound on why certain features were more robust than others.
The process for picking out specific features is inherently difficult, but the paper addressed assumptions and justified when profiling or fuzzing failed.

### 4. Contributions
The paper introduced a systematic way of choosing robust features that can be used to search hidden objects that evade other process scanners.
The tool also outputs a Volatility plugin which makes it readily usable as a prototype for people who want to developing the tool further for different data structures or OS's.

### 5. Clarity
The headings and accurate subheadings correlated closely with the content, which stayed relevant and on-topic.
I rarely found myself wondering what the paragraph was about.
Logical ordering and organization into distinct parts makes each part easier to understand.