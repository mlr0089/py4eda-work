# HW3A Solution - Git and Version Control 

## Part 1: Repository Cloning

I successfully cloned the class repository from `https://github.com/olearydj/INSY6500` to `~/INSY6500/class_repo`.

## Key Commands Used

- `git clone <url>` - create local copy of remote repository
- `git log` - View commit history
- `git remote -v` - Check remote repository connections 

## Part 2: Portfolio Repository Creation

I created my personal course repository with:

- Professional README.md describing the project
Proper .gitignore to exclude unnecessary files
Organized directory structure for homework, projects, and notes

## Understanding Git workflow:

The three-stage workflow:

1. Working Directory: Where I edit files
2. Staging Area: Where I prepare commits with `git add`
3. Repository: Where commits are permanently stored with `git commit`

## Part 3: GitHub Publishing 

Successfully published repository to GitHub:

- Used `git remote add origin` to connect local repo to GitHub
- Used `git push -u origin main` to upload commits
- Verified all files and commits are visible on GitHub

## The Remote Connection 

- `git remote -v` shows the remote URL
- `git push` will send my commits to GitHub
- `git pull` will get updates from GitHub (if changes are made on GitHub)

### Details 

Complete this section with details from your setup:

- Repository URL: https://github.com/mlr0089/py4eda-work
- Output of `git remote -v`:
origin  https://github.com/mlr0089/py4eda-work.git (fetch)
origin  https://github.com/mlr0089/py4eda-work.git (push)
- The output of `git log --oneline`: 
01ebae0 (HEAD -> master, origin/master) Add hw3a solution document
bb95312 Initial commit: Add README and .gitignore

## Questions

### Reflections

#### Question 1:

a) Looking back at my sub-directory from when I took Project Management, I see lots of files with naming conventions such as "Project Charter Russell Draft R001", "Project Chart Russell Draft R003 sans Caitlin and Waleed Sigs", and "Project Charter Final Draft R004". One immediately recognizeable advantage of Git i the ability to review a file's previous revisions within the History of the GitHub interface. Navigating to the History page shows all previous versions of a file that were committed to the Git repository and pushed to GitHub. The History feature allows for easy comparison of the changes made across revisions. Another advatage of Git is the ability to include, short and concise, but descriptive, commit messages. The commit message accompanies the file as a brief description of the initial upload or of the changes from the previously committed revision. For example, instead of naming a file "sans sigs", this could have been included in the commit message. Git also allows for more coordinated and organized collaboration. For the Project Management course previously referenced, I was solely responsible for merging commentary, maintaining the content and sharing the updated documents for each project within my group. Git promotes group member collaboration as no one member has to fear overwriting or deleting significant information as all previous revisions are safely maintained in a repository and can be reverted back to at any time. Lastly, Git eliminates that need to send individual revision files via email or other communciation channels as every revision can be remotely accessed, pulled and updated from the GitHub interface. 

b) One situation from my academic work experience where Git's commit history would have been valuable would have been my mechanical engineering undergraduate senior design captsone project. One core aspect of the project was to design a mechanical billet with various machined features of which dimensions could be analyzed via vision inspection software. Multiple group members providing input into designing a CAD model is complicated enough in-person, but the intricacies of COVID-19 remote learning and social distancing made it even more difficult for concurrent group collaboration. Had we known about Git, each group member to work individually on their own time, pushing their changes to the repository once finished. This ability would have allowed for seamless integration of group member ideas while also always having the safety net of recalling previous revisions, ensuring total group concurrence on all proposed changes. 

#### Question 2:

a) It is important to keep class repo (cloned from the instructor, read-only reference) and my repo (my own work, pushed to GitHub) separate rather than in one repository because there are multiple folders of the same name in both repositories (e.g., homework, projects). If I tried to keep everything in one repository, I couldn't have two folders with the same name and would have to devise a method to differentiate them. If I were to change the name of the folders that were cloned from the course's GitHub page, I imagine this would cause complications when trying to pull and refresh updated content from GitHub. I would also imagine maintaining both the class repo and my repo content in one repository could add complications when trying to push data to GitHub. I don't see a scenario in which would need to publish course reference to my personal GitHub page. If both both personal and course reference material are maintained in the same repository, the entire repository can't be pushed at once, rather, the individual files reflecting my own personal work would have to be specified, potentially adding confusion or requiring additional push commands. All in all, two separate repositories allows for a clean separation of material, mitigating the risk of confusing files.

b) Thinking about future coursework or projects, and how I might organize multiple repositories, I would probably keep all individual assignments in a private folder named after the course or professional project to which they belong. For group projects, I would create a public repository where each group member has both read and write permissions. For reference material, I would probably maintain a public repository where I am the sole individual with write permission, but allow the general public to read all content. I would be sure to devise a strategic naming convention to ensure that my GitHub page can be seamlessly navigated by the public, with clear, descriptive, logical folder locations.

#### Question 3:

a) Comparing the two commit messages, "Add hw3a solution documenting Git workflow and repository structure", is exponentially more useful based on how much more descriptive the message is compared to "udpate". The more descrpitive commit message provides more context to the file and allows for a better understanding of what was committed from breifly reviewing the message. The commit message "update" is extremely vague: What was updated? How much was updated? Was the update significant or rather was it just to fix a typo? This commit amy need to be found again in the future if the source code stops functioning and the author needs to backtrack through the revision history to determine where and when the code broke. 

b) If I were working on a data analysis project over several weeks, I would decide to make commits every time I added significant, valuable content to the project. For example, I would make a commit whenever I completed a major section of the project, or when I completed a significant analysis that provides insightful, relevant information. TO me, what makes a good "unit of work" for a single commit revolves around the amount of value added to the project. It is most likely not worthwhile to flood a revision history with commit messages updating minor typos. This could drastically increase the amount of insignificant commit messages one might need to sort through when reviewing revision history. Rather, to ensure efficient logistics, commits should represent a change that somewhat significantly increased the value of the project (unfortunately, this is subjective and also changes as a project nears completion).

### Graduate Questions
