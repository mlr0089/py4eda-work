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

1. Looking back at my sub-directory from when I took Project Management, I see lots of files with naming conventions such as "Project Charter Russell Draft R001", "Project Chart Russell Draft R003 sans Caitlin and Waleed Sigs", and "Project Charter Final Draft R004". One immediately recognizeable advantage of Git i the ability to review a file's previous revisions within the History of the GitHub interface. Navigating to the History page shows all previous versions of a file that were committed to the Git repository and pushed to GitHub. The History feature allows for easy comparison of the changes made across revisions. Another advatage of Git is the ability to include, short and concise, but descriptive, commit messages. The commit message accompanies the file as a brief description of the initial upload or of the changes from the previously committed revision. For example, instead of naming a file "sans sigs", this could have been included in the commit message. Git also allows for more coordinated and organized collaboration. For the Project Management course previously referenced, I was solely responsible for merging commentary, maintaining the content and sharing the updated documents for each project within my group. Git promotes group member collaboration as no one member has to fear overwriting or deleting significant information as all previous revisions are safely maintained in a repository and can be reverted back to at any time. Lastly, Git eliminates that need to send individual revision files via email or other communciation channels as every revision can be remotely accessed, pulled and updated from the GitHub interface. 

2. One situation from my academic work experience where Git's commit history would have been valuable would have been my mechanical engineering undergraduate senior design captsone project. One core aspect of the project was to design a mechanical billet with various machined features of which dimensions could be analyzed via vision inspection software. Multiple group members providing input into designing a CAD model is complicated enough in-person, but the intricacies of COVID-19 remote learning and social distancing made it even more difficult for concurrent group collaboration. Had we known about Git, each group member to work individually on their own time, pushing their changes to the repository once finished. This ability would have allowed for seamless integration of group member ideas while also always having the safety net of recalling previous revisions, ensuring total group concurrence on all proposed changes. 

