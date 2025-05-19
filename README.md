# VERSION-CONTROL-WITH-GIT
 
*COMPANY* : CODETECH IT SOLUTION

*NAME* :Himanshu Jagannath chavan

*Intern ID*: CT04DK145

*Domain* : DevOps

*Duration* : 4 weeks

*Mentor* : NEELA SANTOSH

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# INDEX.HTML FILE  OF  MAIN 
![Index file v1](https://github.com/user-attachments/assets/4bbf21d5-8908-4867-b293-1f15fc6ceedb)


# CREATING ANOTHER BRANCH NAMED : feature/about
![Image](https://github.com/user-attachments/assets/3091dd35-e3b0-4c05-87a2-bcc49eede94e)


# INDEX.HTML FILE AFTER EDITING
![index file v2](https://github.com/user-attachments/assets/b9c7cf60-4897-4f9d-b5a0-9c6ae066787a)

# CREATING ANOTHER BRANCH NAMED : feature/mission
![Image](https://github.com/user-attachments/assets/258484c5-9c71-4579-a2c8-ada3091948ec)

# INDEX.HTML FILE AFTER EDITING
![Image](https://github.com/user-attachments/assets/cf1e8709-1222-46f3-8af7-bea8c6d78f6e)

# MERGING BRANCHES AND RESOLVING CONFLICT
![Image](https://github.com/user-attachments/assets/4d246b93-c17f-44c0-a982-677f31840a93)

# AFTER RESOLVING CONFLICT INDEX.HTML
![Image](https://github.com/user-attachments/assets/cf1e8709-1222-46f3-8af7-bea8c6d78f6e)


---
step-by-step **general process** done for the Git repository setup, branching, and conflict resolution:


### ✅ Git Workflow: Step-by-Step Process

1. **Initialize a Git repository**

   ```bash
   git init
   ```

2. **Create an initial file and make the first commit**

   ```bash
   echo "Initial Content" > index.html
   git add index.html
   git commit -m "Initial commit"
   ```

3. **Create two branches from `main`**

   ```bash
   git checkout -b feature-A
   git checkout main
   git checkout -b feature-B
   ```

4. **Make different changes to the same line in each branch**

   * In `feature-A`:

     ```bash
     git checkout feature-A
     echo "Change from Feature A" > index.html
     git commit -am "Edit from feature-A"
     ```
   * In `feature-B`:

     ```bash
     git checkout feature-B
     echo "Change from Feature B" > index.html
     git commit -am "Edit from feature-B"
     ```

5. **Merge branches into `main` to generate conflict**

   ```bash
   git checkout main
   git merge feature-A        # Successful merge
   git merge feature-B        # Causes merge conflict
   ```

6. **Resolve the merge conflict**

   * Open `conflict.txt`, manually fix the conflicting lines
   * After editing:

     ```bash
     git add index.html
     git commit -m "Resolved merge conflict between feature-A and feature-B"
     ```

7. **View commit history**

   ```bash
   git log --oneline --graph
   ```

---
