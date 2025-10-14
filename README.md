# CP Lab Quiz Grader

This project is a Python notebook that automatically grades Google Form quizzes for the Cognition & Perception Lab at NYU.

It reads the quiz responses (.csv), compares them to a JSON file with the correct answers, matches student NetIDs with the class roster, and outputs a new CSV file showing each student’s total score and percent correct.

## How to use
1. Export your quiz responses from Google Forms as a `.csv` file.  
2. Create a `.json` file with the correct answers (question → answer).  
3. Make sure the `studentsList.json` file with all NetIDs is one folder above the quiz folder.  
4. Open and run `quizGrader.ipynb`.  
5. A new file (for example `quiz2_grades.csv`) will be created with all scores.

## Example output
| NetID | Name (official) | Total | Percent Correct |
|-------|------------------|--------|-----------------|
| abc123 | Jane Doe | 5 | 100.0 |
| xyz456 | John Smith | 4 | 80.0 |

## Folder structure
cp-lab-2025/
│
├── studentsList.json
└── Quiz2/
├── quiz2_responses.csv
├── quiz2_answers.json
├── quiz2_grades.csv



## Requirements
- Python 3
- pandas
