🧠 Why is pushing directly to main problematic?
Pushing directly to main is risky because it bypasses review and testing. If a team member pushes code with bugs, incomplete features, or accidental deletions, it can break the main product or workflow for everyone. It also makes it harder to track which changes belong to which feature or fix, cluttering the project history.

🌿 How do branches help with reviewing code?
Branches allow each developer to work on a separate feature, bug fix, or experiment without affecting the main codebase. Once work on a branch is done, a pull request (PR) can be opened, letting others review the code, suggest changes, and approve it before merging. This process ensures better code quality, collaboration, and accountability.

⚔️ What happens if two people edit the same file on different branches?
If two people edit the same part of a file on different branches, Git can’t automatically decide which version is correct. This results in a merge conflict when the branches are merged. The team must manually resolve the conflict by choosing which changes to keep. While not ideal, this system ensures that no conflicting work is lost.