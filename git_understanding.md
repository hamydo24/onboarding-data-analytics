1. What is the difference between staging and committing?
- Staging: telling Git what changes you are about to make
- Commiting: taking snapshots of the changes
  + The commit only includes what was staged 

2. Why does Git separate these two steps?
- Commit allows you to select or combine many stages together so we can have a meaningful history of workflow

3. When would you want to stage changes without committing?
- When you make edits to your file, you should stage changes so that you can save them 

=> Git separates staging and committing to let you be intentional about your commits — like curating a playlist instead of dumping every song.

4. Why are PRs important in a team workflow?
Pull Requests (PRs) are important because they allow teams to review code before it’s merged into the main project. This helps catch bugs, enforce coding standards, and ensure that changes are understood and approved by others. PRs also provide a transparent history of why and how changes were made, supporting better collaboration and accountability.

5. What makes a well-structured PR?
A well-structured PR:

Has a clear title and descriptive summary of the changes

Focuses on one feature or fix (not many unrelated changes)

Includes screenshots or test results if needed

References related issues or tickets (e.g., Fixes #42)

Passes all tests and follows coding standards

Anticipates reviewer questions and explains decisions

6. What did you learn from reviewing an open-source PR?
Reviewing an open-source PR taught me how important clarity and communication are in collaborative coding. I saw how maintainers ask thoughtful questions, suggest improvements, and ensure the change aligns with the project’s goals. It also helped me understand how to read code written by others, spot edge cases, and give constructive feedback in a respectful way.




