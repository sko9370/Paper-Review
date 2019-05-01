## Paper Review 6

- Reviewer: Sang Oh
- Paper Title: BlackIoT: IoT Botnet of High Wattage Devices Can Disrupt the Power Grid
- Author: Saleh Soltan, Prateek Mittal, and H. Vincent Poor

### Did you like this paper?  Why?
- What initially caught my attention was the "BlackIoT" description of this topic and the naming of MadIoT.
- I particularly liked how the paper briefly went over the underlying electrical industry concepts to set up the situation for people to understand the implications of this vulnerability better.

### What problem is this paper solving?
- The paper shows the vulnerability of the power grid to attacks by synchronized attacks by attackers.
- It also goes into the possible motivations and purpose behind attacking the power grid.
- Lastly, it explains ways and methods to mitigate this threat.

### What are the strengths of this paper?
- A strength of this paper is that not only does it describe the mechanics of how, but it outlines the possible motivations of why someone would want to attack the power grid.
- It uses real life examples to demonstrate this.
- The simulation also enables the authors to quantify the scale of effects down to the bots per MW.

### What are the main weaknesses in the paper?
- The main weakness of this paper is that the countermeasures are not very thorough or fleshed out.
- More work could have been done to come up with a viable solution; it almost felt like announcing a security vulnerability and not releasing a patch designed to fix it.
- Another weakness is that the numbers generated from this experiment are flawed because they are simulated on a small scale power grid.
- That power grid also doesn't take into account the complete set of security measures already in place.

### Next Steps?
- In the 3.4 Connection to Historical Blackouts, I wouldn't discuss the examples as it was done because it emphasizes that the events happened "because the systems' operators were not prepared for the unexpected initial event," but it does not adequately address how these operators could be better educated for events like this in the future.
- I would extend the paper to come up with viable solutions for this vulnerability, especially from the power grid perspective.
- I think there is room for algorithmic automation to help prevent catastrophic failures in the system, which could prevent problems by not relying on the reaction speed and knowledge of people.
- The vulnerability of IoT seems to relate a lot to bad user practices like passwords because IoT devices are often accessed from the phone or over the internet.
- Further addressing this issue could help greatly resolve the issue of IoT exploitation to achieve power grid manipulation.

## How to Read a Paper

### 1. Category
- It is a research paper describing and analyzing of how IoT botnets could cause immense harm to the power grid.

### 2. Context
- There are a lot of existing papers that discuss the vulnerability of IoT against cyber attacks.
- There is also mention of the use of botnets in recent times to achieve devastating effects.
- Malware that affects power grid systems is also briefly mentioned.
- A lot of concepts behind the operation of power grids is provided to establish a background of basic knowledge for the readers.

### 3. Correctness
- The simulations and results seem sound, but only for use as something to base future experiments on.
- It felt like the simulation did not completely take into account the operations of power grids with respect to security, scale, and method. The problem was simplified.

### 4. Contributions
- The paper contributes to a growing awareness of the vulnerability and risk associated with power grid manipulation through IoT botnets.

### 5. Clarity
- I think the paper is well written in terms of what it contributes and what it does not.
- It clearly states its limitations and what should be explored and researched further.
- Methodology for the simulation is also very clearly stated and explained, making it easy to apply to the overarching concept of power grid vulnerabilities.

https://www.usenix.org/conference/usenixsecurity18/presentation/soltan
