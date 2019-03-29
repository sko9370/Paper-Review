## Paper Review 3

- Reviewer: Sang Oh
- Paper Title: Beyond Precision and Recall: Understanding Uses (and Misuses) of Similarity Hashes in Binary Analysis
- Author: Fabio Pagani, Matteo Dell'Amico, Davide Balzarotti

### Did you like this paper?  Why?

	I liked this paper because algorithms is my favorite CS subject.
	Efficiency and theory is often the subject in most discussions, almost too often.
	This paper provided a different perspective on algorithms by comparing very different fuzzy hashing algorithms,
		and then pitting them against each other in very different and challenging scenarios.
	It was like watching a CS major, IT major, and EE major get graded on boxing, philosophy, and tennis.

### What problem is this paper solving?

	This paper is solving the illusion that ssdeep is the best fuzzy hashing solution for detecting similarity in code.
	By demonstrating in different scenarios that 2 other algorithms, and possibly many others, performed better than ssdeep, readers are convinced to be more open-minded.
	

### What are the strengths of this paper?

	The strengths of this paper are presenting a variety of examples without losing the depth of each scenario.
	The authors picked algorithms that were different enough to present interesting data.
	They also picked adequately interesting and different scenarios that challenged each algorithm.
	This allowed us to see results that were worthwhile and really showed the differences between the algorithms.

### What are the main weaknesses in the paper?

	The main weakness in this paper is the presentation of results.
	Even with a good explanation, the tables and graphs are pretty hard to grasp and understand.
	I think a larger print of a graph that summarizes the results would have been more helpful.
	The rest of the detailed graphs could have gone in the appendix.

### Next Steps?

	Possible future work to this paper would be to test out new fuzzy hashing algorithms.
	
	One of my projects for math modeling plebe year was to combine a consistently underestimating function with a consistently overestimating function.
	I think there may be some room to do something similar with some of the algorithms discussed here or some others that weren't.
	Combining algorithms of different properties may be helpful in situations where the scenario is not as clear and certain as in the paper.
	This may also be an application if the file is corrupted and you have no clue what it might be.

## How to Read a Paper

### 1. Category

	This paper is an analysis and comparison of 4 different fuzzy hashing algorithms in 3 different scenarios.

### 2. Context
	
	There are several fuzzy hashing algorithms that exist.
	ssdeep is considered the industry standard.
	TLSH, sdhash, mrsh are all alternatives and the authors explores reasons why these may perform better than ssdeep in some cases.

### 3. Correctness
	
	Very few assumptions are made, and if they are, they are very robustly supported with details about an algorithm's attributes.
	(ex. tlsh is good at detecting malware similarities because the binaries are very susceptible to minor changes in code that other algorithms can't pick up easily.)
	Statements made about an algorithm's performance in a scenario is supported by the results.

### 4. Contributions
	
	Investigate and explain why a certain fuzzy hashing algorithm works better in some instances than others.
	"...discuss other common problems such as identifying statically-linked libraries,
	detecting the same program across recompilation."

### 5. Clarity
	
	The paper is well written. The paragraphs of writing sticks to the subheadings pretty consistently.
	Good organization of the paper followed.
	An extensive section on history and definition of fuzzy hashing algorithms help set the context of the paper very well.
	I did feel that sometimes the explanations were a bit TOO detailed, but others may appreciate that more than me.
