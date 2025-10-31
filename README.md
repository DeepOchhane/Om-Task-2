# &nbsp;		GitHub



**Configuration Process for Windows**


1. git config --global user.name "Deep Ochhane"
2. git config --global user.email "ochhanedeep93@gmail.com" 





**Set Up Credential Caching (Stores Login Info):**



git config --global credential.helper wincred



**Verify Config:**



git config --list

------------------------------------------------------------------

## 

## Task - 1



###### — Create and Merge Branches

###### 

###### — Create a branch feature-1.

###### 

###### — Add a new file feature.txt and commit.

###### 

###### — Merge it into main.

###### 

👉 Learn: git branch, git checkout, git merge, git branch -d.


Create a new repository on the command line:
---

###### echo "# Om-Task-1" >> README.md

###### git init

###### git add README.md

###### git commit -m "first commit"

###### git branch -M main

###### git remote add origin https://github.com/DeepOchhane/Om-Task-1.git

###### git push -u origin main

### 

### **steps for Task - 1**



###### cmd - git init

###### 

###### cmd - git add README.md

###### 

###### cmd - git commit -m "first commit"

###### 

###### \## cmd - git log --all --graph 

###### 

###### >>>> to check how much commit we did before push or update our changes to repo.

###### 

###### \## create a new branch

###### 

cmd - git branch feature-1

    or
---


\* Directly create and switch to new branch

cmd - git checkout -b feature-1
---

###### 

\## checkout and push changes with new branch 

cmd - git branch branch-name
---

###### 

\## switch branch 

cmd - git checkout branch-name

## we can check and verify our changes once again after switching to the sub branch or new branch 

cmd - git log --all --graph
---

###### 

\## To See the Branch Names and Available branches name

cmd - git branch

## Add url to identify the repo and branch
---


cmd - git remote add origin https://github.com/DeepOchhane/Task-Om-01
---


## Push your branch to GitHub
---

###### 

###### cmd - git push -u origin Testing-task-1  (origin we need to use while pushing our code to the repo first time)



### Steps for Second time:



**Step 1 — Create a new branch feature-1**

use command: git branch feature-1



**git branch feature-1 create and switch to the new branch**



use command: git checkout -b feature-1



**OR Manually**


use command: git checkout feature-1



**Step 2 — add new files, changes and commit:**



use command: git add feature.txt



use command: git commit -m "my feature1/feature.txt changes"




**Step 3 — Switch back to main (or master)**



use command: git checkout main   ***# or git checkout master if your main branch is master***




**Step 5 — Merge feature-1 into main**


use command: git merge feature-1


**Step 6 — Delete the feature branch locally**



use command: git branch -d feature-1







## &nbsp;                       Task - 2

##### **Task Requirements:**

##### 

###### 🎯 Goal

###### 

###### Here we need to perform this task requirements :

###### 

###### Create two branches (feature-A and feature-B) from main.

###### 

###### Modify the same line in both branches (readme.txt).

###### 

###### Merge both branches into main.

###### 

Handle the merge conflict manually.

**Steps: For Resolving conflicts:**
---

###### 

**Step - 1. Creating a feature.txt file with adding some lines**

We can make this file through UI or VS code and add some lines into feature.txt
---

###### 

###### 1st command:--- "git add feature.txt **or git add .**"



###### 2nd command:--- git commit -m "our commit message"

###### 3rd command:--- git push


**Step - 2. Need to edit the same line in both branches:**
---



###### :>> Here we can choose one line to make changes and create the conflict after pushing both of branches changes to main.



###### Creating and switching branch

###### 

###### command:--- git checkout -b feature-1a



###### :>> Make changes on the same line where feature-2 branch changes will make conflicts:



:>> Save the file and run commands for commit and add 

command:--- git add feature.txt
---



###### command:--- git commit -m "koi message"


:>> Switch back to the main branch:

---

###### command:--- git checkout main



**Step - 3. Same changes for feature-2b branch**

Creating and switching branch
---



command:--- **git checkout -b feature-2b**

---

###### :>> Create the changes in same line under feature.txt

###### :>> Run commands: **git add feature.txt** and **git commit -m "same line changes"**

###### :>> Now Switch to main branch to create conflicts use command -- **git checkout main**



###### **Step - 4. Now Merge the Changes from both of branches to see the conflicts:**



:>> Merge Feature-1a changes into main 

use command:--- **git checkout main**
use command:--- **git merge Feature-1a**
---





###### :>> Merge Feature-2b changes into main


use command:--- **git merge Feature-1a**

:>> Now we can see the conflict error message on terminal, output will look like this

{{{C:\\Users\\deep-personal\\Documents\\Git-Practice\\Om-Task-2>git merge Feature-2b
---

###### Auto-merging feature.txt

###### CONFLICT (content): Merge conflict in feature.txt

###### Automatic merge failed; fix conflicts and then commit the result.}}}

###### 

###### **Step - 5. Resolve Conflicts**



###### :>> Now we can see our feature.txt is showing both of changes at on place it here we can see the option to choose

###### &nbsp;   which changes we need to keep**.**



:>> To Resolve this conflicts we need to choose one of the correct branch changes meanwhile we are gonna select the
    Feature-2b branch changes to be Resolve Conflicts.
---



###### :>> After Accept the changes of Feature-2b we need to commit this again with changes after resolving conflicts.



###### use command:--- git add feature.txt

###### use command:--- git commit -m "Conflicts Resolved"



use command:--- git push # finally pushed our change to main.

---





##                         Task - 3

##### **Task Requirements:**


**Task — Push to Remote**
---

##### 

###### Create a repository on GitHub.

###### 

###### Connect local repo with git remote add origin <URL>.

###### 

###### Push code using git push -u origin main.

###### 

###### 👉 Learn: remote setup, push, authentication.





###### **Steps: For Push Local code to Remote and add local Repo to Remote Repo with Origin:**



**Step - 1. Create an empty repository**

:>> Go to the GitHub.com and Create one New Repo Make sure do not choose readme.md 

:>> Click on Create new Repository.

**Step 2 — Initialize Local Repository**
---



###### :>> first we need to initialize the Repo.so git will un



###### Use Command: **git init**



###### **Step 3 — Add Files or Changes** 



###### :>> Here we can select the changes from the specific file or we can add all changes at once with following command.



###### Use Command: **git add . or git add filename.txt**



**Step 4 — Commit the Changes with message** 

---

###### Use Command: **git commit -m "koi message"**

###### 


**Step 5 — Connect Local Repo with Git Remote Repo**
---



###### :>> This Process will help to recognise the actual Repo where our code will be Pushed



###### Use Command: **git remote add origin https://github.com/DeepOchhane/Om-Task-3.git**





**Step 6 — Now we are gonna Push our commit changes to the Remote Repo:**

Use Command: 

:>> Here we can get error with the branch name conflicts, because by default git gives branch name Master for main branch 
    so If we need to change the name of this branch we can run following command or we can use the same name as Master.
---



:>> check your current branch name with this command

---

###### Use Command: git branch



###### :>> Now change the name of current branch Master to main



###### Use Command: **git branch -M main**

###### 

:>> Now we can push our code to the specific Repo but remember we need to use this -u origin commands only once at per Repo
    Meanwhile for the second commit and push we will use simply use git push command to push our changes to the connected 
    Repo. for first commit we will follow this below command:
---

###### 

Use Command: **git push -u origin main**  

---

###### =================================================================





##                         Task - 4

##### **Task Requirements:**





Cloning Friends Repo, Create one Contributor.txt add my name and push back the changes.



Step -1. Fist we will clone the Friends Repo to our Local 

Command: git clone https://github.com/deepdevtest/MavenTesting.git



Step -2. as we are clone it first time and committing something first time we need to initialize the Repo.
Command: git init



Step -3. Create the Contributor.txt and add the contributor name as Deep Ochhane.

&nbsp;- Save the file and go for the next step add and commit.



Step -4. Run git add Contributor.txt and make it commit:



use command: git add .



use command: git commit -m "koi message"



Step -5. Now we need to connect our Local Repo to the Remote repo so our local will know where we want to push our changes we need to always
         follow the same time if we are doing commit first time via local to selected Remote Repo.



Use Command: git remote add origin https://github.com/deepdevtest/MavenTesting.git



Step -6. Push our current changes to the Friends Repo



use command for first time commit: git push -u origin main






## &nbsp;                           Task - 5



### Forking Other GitHub Repo and Push our Changes to them

##### 

##### Step - 1. First Copy Go to the Friends Repo Click on Fork Button Click on Create Fork.

##### 

##### Step - 2. Copy the Code Link to Clone the code to our local Repo

Use Command: - git clone https://github.com/DeepOchhane/test-pr-request-flow.git

Step - 3. verify the clone code was get cloned with forking process and see the origin name
Use Command  - git remote -v
---





##### Step - 4. Need to Change the name as origin to upstream for original Repo of Om Project

##### Use Command: git remote add upstream https://github.com/cod3rjava/test-pr-request-flow.git

##### 

##### Step - 5. Now Fetch the Repo

##### Use Command: git fetch upstream



##### Step - 6. git checkout main



##### Step - 7. git merge upstream main



##### Step - 8. Now make changes or Create any of file and add and commit the changes.



##### WE have Pushed our changes to the remote but still need to create the PR.



##### After Creating the PR we can see the changes into OM's Repo.








&nbsp;                          Task - 6 - Final
Task Requirements:
---



##### Commands for stash: 

1. ##### git status 
2. ##### git diff 
3. ##### git stash # when make change and save the changes temporary.
4. ##### git stash list
5. ##### git stash show
6. ##### git stash pop

##### &nbsp;

##### Step - 1. First we need to Clone our Repo to local 



##### Step - 2. Initialize the Repo

##### Use Command: git init


Step - 3. Connect our local origin/main to Remote/main
---

##### Use Command: git remote add origin https//apni-url.com.git



##### Step - 4. Make changes to the file.



Step - 5. Save the changes with stash.

Run Command: git stash or -->
---



##### Step - 6. Run git stash -m "koi message stash related"



##### Run Command: git stash -m "First Stash"



##### Step - 7. Check the list of your current stash.

##### Use Command: git stash list

##### 

##### Step - 8. Now apply your last changes with stash Run $git stash apply

##### Use Command: git stash apply

##### 

##### Step - 9. If we want to apply particular 1st or 3rd stash from the list we need to Run this

##### &nbsp;         Command

##### Use Command: git stash apply stash@{3/1}

##### 

Step - 10. To See our stash pending commits

Use Command: got stash pop

Step - 11. Push our changes to the main branch.
---

Use Command : git push 		# to update our changes to remote main.


---


