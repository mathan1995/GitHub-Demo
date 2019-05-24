# GitHub-Demo
---
## 1. Please follow these steps **always**, whenever you push a file.
- Only add your **changed file**
  - git add TestDocument.txt
- Commit your changes (only after surely verified) with a meaning full message. 
  - git commit -m "My name with a short description added"
- You should pull from remote to your local, Then only you won't get conflict.
  - git pull
- If you get any conflict, first resolve it. **Carefully watch the changes**
  - **Repeat from the first step.**
- Finally push your changes
  - git push
  
---

## 2. Tips and Commands for easy use of GitHub.
- If you done some changes in a **wrong branch** you can bring the changes to the **correct branch**, if you did not commit it. Try the following steps **CAREFULLY**.
  1. Checkout master branch
      - git checkout master
  2. Do some changes in Test Document.
  3. Now bring back the changes from master to the branch final-try.
      - git stash
        - You are temperorily get out all the changes and save them in a temperoy memory, from master branch files
      - git checkout final-try
        - Changing the branch where you want the changes actually.
      - git stash apply
        - Applying all the changes which you brought out from the master, (Which is in the temperory memory).
        
 **Successfully you brought the changes form master to final-try** 
 
 - If you add a wrong file accidently which has changes, you can remove it. Try the following steps.
    - git add <Changed wrong file name>
      - You are adding a wrong file which has changes.
    - git reset <Changed wrong file name>
      - You are removing the added wrong file.
      
 **Successfully you removed an unwanted file**
 
 ---
