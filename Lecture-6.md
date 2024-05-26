
#### Introduction

**Q1:** **What problem does version control address with multiple document versions like EssayFinal, EssayFinal2, etc.?**  
<details>
<summary>Answer</summary>
Version control helps manage multiple versions of a document, keeping track of changes, and preventing confusion from having many versions like EssayFinal, EssayFinal2, etc.
</details>

#### Version Control System (VCS)

**Q2:** **What are the key challenges addressed by a version control system?**  
<details>
<summary>Answer</summary>
1. Collaboration
2. Version management
3. Data backup
4. Restoring previous versions
5. Change tracking
</details>

**Q3:** **Define Version Control System (VCS).**  
<details>
<summary>Answer</summary>
VCS, also known as source control or revision control, is a system that tracks the progress of code through its lifecycle and multiple iterations, maintaining a record of every change, including authorship, timestamp, and details.
</details>

#### Types of Version Control Systems

**Q4:** **What are the differences between centralized and distributed version control systems?**  
<details>
<summary>Answer</summary>
- **Centralized VCS**: Stores files in a central repository; users work with the same repository; single point of failure.
- **Distributed VCS**: Clients fully mirror the repository; offline operations allowed; network connection needed only for publishing changes.
</details>

**Q5:** **What is a lock-based version control system?**  
<details>
<summary>Answer</summary>
A lock-based VCS uses file locking to manage concurrent access to files and resources, preventing conflicting changes by allowing only one user to edit a file at a time.
</details>

**Q6:** **What is an optimistic version control system?**  
<details>
<summary>Answer</summary>
An optimistic VCS allows users to work in private workspaces and submit changes to the server, which merges them to avoid conflicts.
</details>

#### Benefits of Version Control

**Q7:** **List some benefits of using a version control system.**  
<details>
<summary>Answer</summary>
1. Streamline merging and branching
2. Examine and experiment with code
3. Track changes
4. Access modification history
5. Automated backups
6. Regulatory compliance
</details>

#### Git and GitHub

**Q8:** **What is the difference between Git and GitHub?**  
<details>
<summary>Answer</summary>
- **Git**: An open-source VCS created in 2005 for Linux development, tracking file changes.
- **GitHub**: A company providing tools that integrate with Git, enhancing collaboration and code sharing.
</details>

**Q9:** **Do you need GitHub to use Git?**  
<details>
<summary>Answer</summary>
No, Git can be used without GitHub, but GitHub enhances sharing and collaboration.
</details>

#### How Git Works

**Q10:** **How does Git store file changes?**  
<details>
<summary>Answer</summary>
Git stores files and their development history in a local repository. Changes are saved as commits, which are snapshots of files identified by unique hashes.
</details>

**Q11:** **What types of files are included in a Git repository?**  
<details>
<summary>Answer</summary>
Source files, build scripts, documentation, and resource files. Generated files (e.g., `.o`, `.dll`, `.class`, `.exe`) are excluded.
</details>

#### Branching

**Q12:** **What is a branch in Git?**  
<details>
<summary>Answer</summary>
A branch is a parallel copy of the source code, allowing developers to work on features independently. Changes are merged into the main version (master branch) after completion.
</details>

#### Commit

**Q13:** **Describe the three states of files in Git.**  
<details>
<summary>Answer</summary>
1. **Modified**: Changes made but not staged.
2. **Staged**: Changes marked for inclusion in the next commit.
3. **Committed**: Changes stored in the Git database.
</details>

#### Installing Git and Configuring the Environment

**Q14:** **How do you install Git on a computer?**  
<details>
<summary>

Answer</summary>
Use the command `sudo apt-get install git`.
</details>

**Q15:** **How do you verify the installation of Git?**  
<details>
<summary>Answer</summary>
Use the command `git --version`.
</details>

**Q16:** **How do you configure your Git username and email?**  
<details>
<summary>Answer</summary>
Use the commands:
- `git config --global user.name "Your Full Name"`
- `git config --global user.email you@somewhere.com`
</details>

#### Creating a Project

**Q17:** **What are the steps to create a new Git project?**  
<details>
<summary>Answer</summary>
1. Create a directory: `mkdir tmp`
2. Navigate into the directory: `cd tmp`
3. Create a project directory: `mkdir test1`
4. Navigate into the project directory: `cd test1`
5. Initialize the Git repository: `git init`
</details>

#### Stage and Commit Example

**Q18:** **How do you stage a file in Git?**  
<details>
<summary>Answer</summary>
Use the command `git add <filename>`.
</details>

**Q19:** **How do you stage all existing files in Git?**  
<details>
<summary>Answer</summary>
Use the command `git add -A`.
</details>

**Q20:** **How do you commit changes in Git?**  
<details>
<summary>Answer</summary>
Use the command `git commit -m "message"`.
</details>

This comprehensive QnA question bank covers all the relevant content from Lecture 6 on Unix and Shell Scripting, including detailed analysis and examples from the images provided in the lecture slides. If you need any more questions or further details on specific topics, let me know!
