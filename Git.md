---
date: 2024-12-15
tags: 
link:
---

## Version Control

version control is like an `epic` save button that allow us to revert back to previous version of a project or a file. It is used to keep track of the versions of  our project 

### Local
![Pasted image|300](images/Pasted%20image%2020241215121915.png)


### Centralized
![Pasted image|300](images/Pasted%20image%2020241215122127.png)

### Distributed
![Pasted image|300](images/Pasted%20image%2020241215122158.png)

### Comparison Table

| Feature             | Local VCS   | Centralized VCS        | Distributed VCS |
| ------------------- | ----------- | ---------------------- | --------------- |
| **Repository**      | Local only  | Central server         | Local + Central |
| **Collaboration**   | None        | Yes                    | Yes             |
| **Offline Access**  | Full access | Limited                | Full access     |
| **Fault Tolerance** | Low         | Low (server-dependent) | High            |
| **Examples**        | RCS, SCCS   | SVN, CVS               | Git, Mercurial  |


## Orgin

### **Summary of 1.2: A Short History of Git**

- **Origin**: Git was created in 2005 by Linus Torvalds, the creator of Linux, after the Linux community lost access to the proprietary DVCS BitKeeper.
- **Design Goals**:
    - Speed
    - Simple design
    - Strong support for non-linear development (e.g., branches)
    - Fully distributed
    - Efficiency with large projects like the Linux kernel.
- **Features**: Git retains its initial goals, providing speed, efficiency, and a powerful branching system.

---

### **Summary of 1.3: What is Git?**

- Git is a distributed version control system that operates differently from traditional VCSs like CVS and Subversion.
- **Key Features**:
    1. **Snapshots, Not Differences**: Git stores project data as snapshots (complete states) instead of changes (deltas).
    2. **Local Operations**: Most operations happen locally, making Git fast and functional offline.
    3. **Data Integrity**: Uses SHA-1 checksums to ensure data integrity and prevent corruption.
    4. **Append-Only Nature**: Most actions in Git add data rather than modifying or deleting it, ensuring changes are recoverable.

---

### **Summary of 1.4: The Three States of Git**

- Git organizes files into three main **states**:
    
    1. **Modified**: Files changed but not yet staged.
    2. **Staged**: Changes prepared for the next commit.
    3. **Committed**: Changes stored permanently in the Git database.
- **Key Components**:
    
    - **Working Tree**: The current checked-out files you modify.
    - **Staging Area**: Prepares files for the next commit.
    - **Git Directory**: Stores the metadata and database of the project.
- **Workflow**:
    
    1. Modify files in the working tree.
    2. Stage the changes.
    3. Commit the changes to the Git directory.
- **Usage**: The command line provides the most comprehensive Git functionality, making it essential to understand its usage.
