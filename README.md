# **📘 Git \+ GitHub Training Session**

### **Version Control for DID-Inc Server Scripts**

---

## **🟩 1\. Introduction**

### **Purpose of Git**

* Track every change made to our server scripts

* Maintain a full version history

* Prevent accidental overwrites

* Make collaboration safe and organized

* Provide an easy rollback mechanism if a script breaks

**Why this matters:**  
 Git gives us structure, stability, and protection for all automation that runs the company.

---

## **🟦 2\. What Are Git & GitHub?**

### **Git**

A version control system installed on the computer.  
 It tracks changes and saves versions of files.

### **GitHub**

A cloud platform that stores the repository online.  
 It acts as the central “source of truth.”

### **Relationship**

Computer (Git) → push → GitHub (online repo)  
GitHub → pull → Computer or Server  
---

## **🟩 3\. The Git Workflow (High-Level)**

Git has three main zones:

* **Working Directory** – where files are edited

* **Staging Area** – where selected changes are prepared

* **Local Repository** – where commits are saved

* **Remote Repository (GitHub)** – central online copy

### **Core Workflow**

pull → add → commit → push  
---

## **📸 Git as Photography — Mental Model**

┌───────────────────────────────────────────────────────────────┐  
│                      📸 GIT AS PHOTOGRAPHY                     │  
│             A Simple Mental Model for Understanding Git         │  
└───────────────────────────────────────────────────────────────┘

### **📂 WORKING DIRECTORY**

**“Setting up the scene”**

* This is where you freely edit files

* Add, remove, rewrite, reorganize

* Nothing is saved yet — you’re preparing the shot

---

### **🟨 STAGING AREA → `git add`**

**“Choosing what will be in the photo”**

* You select the changes you want to save

* Maybe you changed 10 files, but only want 2 in the photo

* The staging area lets you pick *exactly what will be committed*

---

### **📷 COMMIT → `git commit -m "message"`**

**“Taking the photo”**

* A permanent snapshot of the staged files

* Saved locally on your machine

* You can always return to this exact point in time

* Like hitting the shutter button

---

### **☁️ PUSH → `git push`**

**“Uploading the photo to the cloud (GitHub)”**

* Sends the snapshot to the shared repository

* Updates the official copy everyone uses

* GitHub becomes the team photo album of all versions

---

### **⭐ COMPLETE ANALOGY SUMMARY**

WORKING DIRECTORY   \= Setting up the scene  
STAGING AREA        \= Choosing what’s in the photo  
COMMIT              \= Taking the photo  
PUSH                \= Uploading the photo to GitHub

**Use this mental model to remember the Git workflow:**

pull → add → commit → push  
---

## **🟦 4\. Installation & Accounts**

### **Requirements:**

* Git Bash installed on local PC (default installation options are fine)

* Personal GitHub account using company email

* Access to private company repositories

Git Bash will be used to run Git commands on the local machine.

---

## **🟩 5\. Creating a GitHub Repository (Demonstration)**

This section is demonstrated live:

### **Steps shown:**

* Create a new repository on GitHub

* Set visibility to **Private**

* Keep default settings

* Copy repository URL for cloning

---

## **🟦 6\. Basic Git Commands (Demonstration \+ Participation)**

### **1\. Clone**

Creates a local copy of the repository.

git clone \<repo-url\>  
---

### **2\. Status**

Shows what changed, what is staged, and what is committed.

git status  
---

### **3\. Pull**

Updates the local repository with the latest changes from GitHub.

git pull

**Golden Rule:** Always run `git pull` before making changes.

---

### **4\. Add**

Moves modified files into the staging area.

git add .  
---

### **5\. Commit**

Saves a snapshot of staged files in the local repository.

git commit \-m "Description of changes"  
---

### **6\. Push**

Uploads the commit to GitHub so both team members see it.

git push  
---

## **🟩 7\. Hands-On Exercise (Performed by Participant)**

### **Steps:**

1. Clone repository locally

2. Run `git pull`

3. Open any file and make a small edit

4. Run `git status`

5. Stage changes with `git add .`

6. Commit with `git commit -m "message"`

7. Push with `git push`

8. Verify changes appear on GitHub

---

## **🟦 8\. Navigating GitHub’s UI**

### **Key areas demonstrated:**

* Viewing commit history

* Comparing changes (diff)

* Viewing file history

* Browsing the repository

* Searching files

This helps with troubleshooting and reviewing script changes.

---

## **🟥 9\. Important Guidelines**

### **Do Not Use (We won’t need these):**

* Branching

* Merging

* Rebasing

* Resetting

* Stashing

* Force pushing

The workflow is intentionally kept simple to avoid unnecessary complexity.

---

## **🟧 10\. How the Server Will Stay Updated**

### **Overview:**

* A safe automated system will run on the server

* It will periodically run `git pull`

* It will only pull when no local changes exist

* This prevents:

  * Overwriting local edits

  * Creating merge conflicts

  * Breaking production scripts

GitHub becomes the single source of truth for all DID-Inc server automation.

---

## **🟩 11\. The Standard Workflow to Always Follow**

1\. git pull  
2\. Edit files  
3\. git add .  
4\. git commit \-m "message"  
5\. git push

### **Following this workflow ensures:**

* No conflicts

* No lost work

* No surprises

* A clean and accurate history

---

## **🟦 12\. Wrap-Up**

After this session, each participant should understand:

* What Git and GitHub are

* How repositories work

* How to clone, pull, add, commit, and push

* How to view changes on GitHub

* How the server auto-update process works

* The expected workflow for updating scripts

Support is available for any Git-related questions as the team begins using this workflow.

