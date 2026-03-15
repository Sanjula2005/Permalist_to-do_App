DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test
$ git config --global user.name "Sanjula2005"

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test
$ git config --global user.email "sanjulasudhindra12@gmail.com"

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test
$ git init
Initialized empty Git repository in C:/Users/DELL/Desktop/test/.git/

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git add .

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git commit -m "Initial commit"
[master (root-commit) 52eb10f] Initial commit
 1 file changed, 1 insertion(+)
 create mode 100644 x.py

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git remote add origin https://github.com/Sanjula2005/test.git

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 228 bytes | 114.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Sanjula2005/test.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git log
commit 52eb10fec7538fc6ddd0835bdca376befc6fd5f0 (HEAD -> master, origin/master)
Author: Sanjula2005 <sanjulasudhindra12@gmail.com>
Date:   Sun Mar 15 19:14:52 2026 +0530

    Initial commit

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git add .

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git commit -m "second commit"
[master 3962170] second commit
 1 file changed, 1 insertion(+), 1 deletion(-)

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git push -u origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 263 bytes | 263.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Sanjula2005/test.git
   52eb10f..3962170  master -> master
branch 'master' set up to track 'origin/master'.

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git reset --hard HEAD~1
HEAD is now at 52eb10f Initial commit

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ GIT LOG
git: 'LOG' is not a git command. See 'git --help'.

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$ git log
commit 52eb10fec7538fc6ddd0835bdca376befc6fd5f0 (HEAD -> master)
Author: Sanjula2005 <sanjulasudhindra12@gmail.com>
Date:   Sun Mar 15 19:14:52 2026 +0530

    Initial commit

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test (master)
$































DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2
$ git clone https://github.com/Sanjula2005/dev.git
Cloning into 'dev'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2
$ cd dev

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ touch file.txt


DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ ^C

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ ^C

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ ^C

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ git branch two

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ git checkout two
Switched to branch 'two'

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (two)
$ git branch
  master
* two

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (two)
$ git add .

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (two)
$ git commit -m "feature added"
[two 1783045] feature added
 1 file changed, 1 insertion(+), 1 deletion(-)

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (two)
$ git push origin two
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 279 bytes | 279.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'two' on GitHub by visiting:
remote:      https://github.com/Sanjula2005/dev/pull/new/two
remote:
To https://github.com/Sanjula2005/dev.git
 * [new branch]      two -> two

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (two)
$ git diff main two
fatal: ambiguous argument 'main': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (two)
$ git diff master two
diff --git a/index.html b/index.html
index a517333..7a64540 100644
--- a/index.html
+++ b/index.html
@@ -6,6 +6,6 @@
     <title>Document</title>
 </head>
 <body>
-    <h1> Hello there!!</h1>
+    <h1> Hello!</h1>
 </body>
 </html>
\ No newline at end of file

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (two)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ git add .

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ git commit -m "main change"
[master 971c55e] main change
 1 file changed, 1 insertion(+), 1 deletion(-)

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ git push origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 292 bytes | 292.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Sanjula2005/dev.git
   4497bbe..971c55e  master -> master

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ git diff master two
diff --git a/index.html b/index.html
index 71df9e4..7a64540 100644
--- a/index.html
+++ b/index.html
@@ -6,6 +6,6 @@
     <title>Document</title>
 </head>
 <body>
-    <h1> Hello there!! how are you?</h1>
+    <h1> Hello!</h1>
 </body>
 </html>
\ No newline at end of file

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ git merge two
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master|MERGING)
$ ^C

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master|MERGING)
$ git merge two
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master|MERGING)
$ ^C

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master|MERGING)
$ git add .

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master|MERGING)
$ git commit -m "resolved"
[master dba8819] resolved

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ git merge two
Already up to date.

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ git diff master two
diff --git a/index.html b/index.html
index a717151..7a64540 100644
--- a/index.html
+++ b/index.html
@@ -6,7 +6,6 @@
     <title>Document</title>
 </head>
 <body>
-    <h1> Hello there!! how are you?</h1>
-
+    <h1> Hello!</h1>
 </body>
 </html>
\ No newline at end of file

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$ git log
commit dba8819a6c36cdaa278b856f1b637f84c6130c01 (HEAD -> master)
Merge: 971c55e 1783045
Author: Sanjula2005 <sanjulasudhindra12@gmail.com>
Date:   Sun Mar 15 19:32:55 2026 +0530

    resolved

commit 971c55e903ba0d90092fda551c5c24ab6085bece (origin/master, origin/HEAD)
Author: Sanjula2005 <sanjulasudhindra12@gmail.com>
Date:   Sun Mar 15 19:30:09 2026 +0530

    main change

commit 17830450604388c3cc7ef2c6f594cfc03ac847c8 (origin/two, two)
Author: Sanjula2005 <sanjulasudhindra12@gmail.com>
Date:   Sun Mar 15 19:27:23 2026 +0530

    feature added

commit 4497bbe3a91dfd423fa43256193e408db8178a6f
Author: Sanjula2005 <sanjulasudhindra12@gmail.com>
Date:   Sun Mar 1 18:16:56 2026 +0530

    Initial commit

DELL@LAPTOP-7F0R149E MINGW64 ~/Desktop/test2/dev (master)
$








































Below is a **clean lab-record format** for your experiment.

---

# **Experiment 3: Integrating GitHub with Jenkins for CI/CD Pipeline**

## **Aim**

To demonstrate the process of integrating a **GitHub** repository with **Jenkins** to automate project execution in a **CI/CD Pipeline**.

---

# **Requirements**

### Hardware

* Computer with minimum **8 GB RAM**
* Internet connection

### Software

* **Git**
* **GitHub** account with repository
* **Jenkins**
* **Java** / **Python**
* **Ngrok** (for webhook testing)

---

# **Step 1: Install and Setup Jenkins**

1. Download **Jenkins** from the official website.
2. Install Jenkins on the system.
3. Open a browser.
4. Go to:

```
http://localhost:8080
```

5. Jenkins will ask for **Administrator Password**.
6. Open the file:

```
C:\ProgramData\Jenkins\secrets\initialAdminPassword
```

7. Copy the password and paste it into the Jenkins setup page.
8. Click **Continue**.
9. Select **Install Suggested Plugins**.
10. Create the **Admin User**.
11. Finish the setup and open the **Jenkins Dashboard**.

---

# **I. Manual Build Creation**

### Step 1: Create a Job

1. Open **Jenkins** dashboard.
2. Click **New Item**.
3. Enter the **Project Name**.
4. Select **Freestyle Project**.
5. Click **OK**.

---

### Step 2: Configure GitHub Repository

1. Go to **Source Code Management**.
2. Select **Git**.
3. Enter the repository URL from **GitHub**.

Example:

```
https://github.com/username/repository-name.git
```

---

### Step 3: Add Build Step

1. Scroll to **Build**.
2. Click **Add Build Step**.
3. Select **Execute Windows Batch Command**.

Example commands:

For Python:

```
python file.py
```

For Java:

```
javac file.java
java file
```

Or simple test:

```
echo Hello Jenkins
```

---

### Step 4: Save and Run

1. Click **Save**.
2. Click **Build Now**.
3. Jenkins executes the project automatically.

---

# **II. Scheduled Build (Using Poll SCM)**

### Step 1: Create a New Jenkins Job

1. Click **New Item**.
2. Enter project name.
3. Select **Freestyle Project**.
4. Click **OK**.

---

### Step 2: Connect GitHub Repository

1. Go to **Source Code Management**.
2. Select **Git**.
3. Enter repository URL.

---

### Step 3: Enable Poll SCM

1. Scroll to **Build Triggers**.
2. Select **Poll SCM**.
3. Enter schedule:

```
* * * * *
```

---

### Step 4: Add Build Step

1. Go to **Build**.
2. Click **Add Build Step**.
3. Select **Execute Windows Batch Command**.

Example:

```
echo Running build
python file.py
```

---

### Step 5: Save the Job

1. Click **Save**.
2. Now Jenkins checks the repository regularly.

If a change occurs in **GitHub**, Jenkins **automatically starts a build**.

---

# **III. Event-Based Automatic Build Using Webhooks**

### Step 1: Create Jenkins Job

1. Click **New Item**.
2. Enter project name.
3. Select **Freestyle Project**.
4. Click **OK**.

---

### Step 2: Configure Git Repository

1. Go to **Source Code Management**.
2. Select **Git**.
3. Enter GitHub repository URL.

---

### Step 3: Enable GitHub Trigger

1. Scroll to **Build Triggers**.
2. Select:

```
GitHub hook trigger for GITScm polling
```

---

### Step 4: Run Ngrok

Install **Ngrok**.

Run command:

```
ngrok http 8080
```

This exposes Jenkins to the internet.

Example URL:

```
https://abcd1234.ngrok.io
```

---

### Step 5: Add Webhook in GitHub

1. Open repository in **GitHub**.
2. Go to **Settings**.
3. Click **Webhooks**.
4. Click **Add Webhook**.

Enter:

Payload URL:

```
http://ngrokURL/github-webhook/
```

Example:

```
https://abcd1234.ngrok.io/github-webhook/
```

Click **Add Webhook**.

---

### Step 6: Test the Pipeline

1. Make a change in the repository.
2. Push the code to **GitHub**.
3. Webhook sends a request to **Jenkins**.
4. Jenkins automatically triggers the build.

---

# **What is Poll SCM?**

**Poll SCM** is a Jenkins feature that **periodically checks the Source Code Management repository for changes**.

If Jenkins detects any change in the repository, it **automatically starts a build process**.

Example schedule format:

```
* * * * *
```

This means Jenkins checks the repository **every minute**.

---

# **Result**

Successfully integrated **GitHub** with **Jenkins** to automate builds using **manual, scheduled, and webhook-based CI/CD pipeline methods**.

---

If you want, I can also give **very short exam-friendly definitions of Jenkins, CI, CD, Poll SCM, and Webhooks** (these are commonly asked viva questions for this experiment).
