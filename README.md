# cs50-Runoff
A C program that simulates an election using the instant-runoff voting system (also known as ranked-choice voting). Built as part of CS50x (Introduction to Computer Science by Harvard University).

📖 Overview

The program collects a list of candidates and allows voters to rank them in order of preference. During each round of counting:
	1.	Votes are tallied based on each voter’s highest-ranked candidate still in the race.
	2.	The candidate with the fewest votes is eliminated.
	3.	Votes for eliminated candidates are redistributed according to the next preference.
	4.	The process repeats until a candidate has more than 50% of the votes, or a tie occurs.

This simulates a real-world ranked-choice election system.

Example:
	•	Input: 3 candidates (Alice, Bob, Charlie)
	•	Voter 1 ranks: Alice > Bob > Charlie
	•	Voter 2 ranks: Bob > Charlie > Alice
	•	Voter 3 ranks: Charlie > Alice > Bob
	•	Output: Winner determined through runoff rounds

🛠 Features
	•	Implements instant-runoff (ranked-choice) voting in C.
	•	Supports multiple candidates and multiple voters.
	•	Handles ties and elimination correctly.

🚀 How to Run
	1.	Compile the program: make runoff
  2.  Run the program with candidate names: ./runoff Alice Bob Charlie
  3.  Enter each voter's ranked preferences when prompted.

📂 Files
	•	runoff.c – main source code
	•	README.md – project documentation
