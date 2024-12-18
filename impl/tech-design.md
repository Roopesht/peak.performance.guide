# Technical design of Peak performance


## Components to be used
python
Langchain

## User story to be implmented
### Flow #1
Show the Paraphrased version of the Goal and challenges

Rephrase the goal and the challenges for more clarity 



### Flow #2
Provide the best solution for the challenge, 
The user can request for another solution
Finally user can accept one of the solution

#### Prompt:
Here is the goal and the challenge. Please suggest a solution. The output should be in the below format: 
{"output": "the solution in 50 words or more", "shortform": "The solution in 10 words or less"}

Goal: A CBSE 10th standard student scoring currently 60%, aiming for 80%

Challenge: He needs around 4 hours to prepare on each lesson, how ever he does not have so much of time. He has approxmately 240 hours, but he has to cover 60 lessons, and also need time for revision.

Please exclude the below solutions, as these are already tried.
Sol 1: Prioritize lessons, shorter sessions, and active revision methods.


### Flow #3
The prescribed by the system  can be modified by the user. The solution is further rephrased and cleaned by the sytem and get the user's acceptance

#### Prompt:
Here is the goal challenge and solution. Please validate the solution, and provide the cleaned up version.

Goal: A CBSE 10th standard student scoring currently 60%, aiming for 80%

Challenge: He needs around 4 hours to prepare on each lesson, how ever he does not have so much of time. He has approxmately 240 hours, but he has to cover 60 lessons, and also need time for revision.

Solution: The student should adopt a strategic approach by summarizing lessons into concise notes, focusing on NCERT questions and frequently asked exam topics. Incorporate group discussions, audio-visual aids, and teaching peers to reinforce learning. Allocate 70% of time to lessons and 30% to revisions, utilizing flashcards for quick reviews.


### Flow #4
Convert the solution to plan (actionable steps)

The user can accept and add more steps as needed

#### Prompt:
Here is the goal, challenge and the solution.  Please provide the actionable steps. The output should be in the below format: 
[{"step": "Actual step in words", "slno": "serial number", "recurring": "y/n", "recurringinterval": "d/h/wd/mon"}]

Goal: A CBSE 10th standard student scoring currently 60%, aiming for 80%

Challenge: He needs around 4 hours to prepare on each lesson, how ever he does not have so much of time. He has approxmately 240 hours, but he has to cover 60 lessons, and also need time for revision.
Solution: The student should adopt a strategic approach by summarizing lessons into concise notes, focusing on NCERT questions and frequently asked exam topics. Incorporate group discussions, audio-visual aids, and teaching peers to reinforce learning. Allocate 70% of time to lessons and 30% to revisions, utilizing flashcards for quick reviews.

