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

#### Question 1:

a) It was valuable to commit the README and .gitignore together first because these files serve to establish the infrastructure of the repository rather than include significant value added content. The README and .gitignore files set the stage for the content that will and will not be tracked in the Git repository, rather than just immediately adding assignment/project specific files. hw3a-solution.md is value added content that accopmlishes a specific task that the README file explains will be included in the repository. Additionally, had we committed everything at once, we would have lost the individual, granualr traceability of the hw3a-solution.md file commit. Separating the commits for the setup work vs. the task-specific/value-added work provides a cleanear, easier to understand workflow that also supports troubleshooting and future revision history review. 

b) If I was working on a homework assignment over sevral days, I would commit the code to load the data and the update to the README file. Wiriting code to load data is significant value-added content of which it could be useful to track the revision. Updating the README file completes a new version of the file, so this too should also be committed now so outside parties have the latest information pertaining to the project. Fixing a typo in a comment is most likely an insiginficant change that does not warrant it's own commit message (unless the typo misrepresents the analysis). This change can most likely wait to be pushed with a more significant change to the file to avoid over-saturating the file history with minute, non-value added changes. Getting half-way done on a new analysis function is an interesting situation. To me, it depends on the type of content provided in the half-finished analysis. Has the work that's been done primarily been focused on setting the foundation of the analysis, or are results available from which informed decisions can be made? If the former, I would probably wait before commiting until some form of results are availalbe, if the later, I would commit and start tracking the revision of the anlysis file. Staging supports this decision making process as the workflow requires specific files be added to the staging area, so it doesn't necesarrily make sense to add an "incomplete" file to the staging area, especially if it is actively being worked. However, it does make sense to add files that have been completed, updated, or do not need to worked any futher. Staging also acts as a safety net, allowing for a complete review before commiting all files in the staging area, and making sure all staged files make sense to commit under the same commit message. 

c) Git status shows you if your branch is up to date with "origin/master", what changes are not staged for commit, and what changes are staged for commit. In essence, it shows you what files have changed and if they are ready to be committed or not. Git status can serve as a "tracker" of what files you are planning on staging and committing and what files you are maintaining as untracked. Git status should be used consistently in your workflow, as it clearly shows you what bin each file is in. I would specifically use it after completing significant work in a file, or when wraping up for the day, as these are two points along the workflow that it would be useful to see what changes are stagged, tracked and untracked and provides an natural decision point on whether these files should be committed or not. 

#### Question 2:

a) From my lecture notes, we described distributed as meaning "Every repository is a complete mirror - not client-server model". This means that my local "class repo" folder is an exact replicate of the INSY6500 class_repo repository from Dr. O'Leary's GitHub page. I have complete autonomy over the duplicated files on my local machine, but at the time of cloning the repository, the files were exact matches to those that were published on Dr. O'Leary's INSY6500 GitHub repository. Pertaining to "my repo", I also have complete autonomy over the files in this repository, but when I commit them to Git, Git maintains an exact replicate of the file at the time it was committed. This is different from Google Drive as files stored in this repository can be accessed and editted by anyone with the appropriate permissions. Once a file is updated, there is no reverting back to a previous revision, as there is only one file.

b) Being able to work on your local repository without internet connection is valuable to developers because it increases flexibility while also eliminating a common source of failure. Since internet is not a gate to working i nGit, developers can work anywhere they have their local machine without having to worry about a stable wifi connection. Google Drive, for example, requires an internet connection in order to access and edit files. If the internet connection crashes while workingin Google Drive, updates could be lost and the developer would be constrained on the amount of work they would be able to continue doing. This would not be an issue when working in Git as changes can be tracked locally and then pushed to GitHub when a stable internt connection is re-established, allowing the developer to continue work without interruption. 

c) Git clone creates a subdirectory of the cloned repository, downloading all content to your local device. Git pull allows a user to update one's local copy of a cloned subdirectoy with the latest updates that were published to Git/GitHub, allowing the user to stay current with the public developer's work. Git push allows a developer to publish his/her work to GitHub, becoming accessible to the public. I can pull from "class repo" because it is a public repository that I can access. I cannot publish to "class repo" on Dr. O'Leary's GitHub page because the owner of the repository has blockers that prohibit the public from editing his publicaly accessible repository. My "my repo" repository allows me to push and pull from it because it is my public repository to which I have all read/write (push/pull) permissions. 

#### Question 3:

a) First and foremost, when deciding what to commit, I need to remember that my GitHub page is a public repository that theoretically can be accessed by anyobdy at anytime. I need to ensure that what I publish appropriately represents me personally and professionally. I should specifically consider if the work I am thinking of publishing demonstrates critical data anlysis skills that are showcase worthy. I think an easy solution to balancing showing ones work process versus presenting polished, final product is having two separate folders, one for work-in-process and one for finished product. This way, my work process and the steps I took to reach a final product can be showcased, but I also have a clear, distinct folder demonstrating what I consider to be final, deliverable product. 

b) A README for an open-source project most likely includes information or recommended guidelines on how to use the code for personal or professional purposes. It is most likely more focused on the code itselg rather than the individual or the general work of the individual who created the code. A README file for a portfolio repository should be more focused on the author and the content the author creates that is maintained in the repository rather than the underlying theory of the files contained in the repository themselves. I imagine an effective README for a portfolio repository really emphasizes the strengths of the author, and provides high-level overviews of how those strengths are implemented in the repository content. A personal README should be more visually appealing, as it is more representative of the author him/herself, and should be focused on showcasing the author's skills, while an open-source project README should be clear, concise and focused on describing how the code can be effectively and efficiently used by a wide variety of audiences. 

c) Building a public portfolio during my coursework rather thanw aiting until I am job searching is valuable because it allows me to build and showcase my skills as I am developing them rather than having to recall them after I have completed this course and maybe have not used the course material in some time. Additionally, it will be much easier to point t ospecific examples that are already published on my GitHub page during a job interview rather than having to describe vague scenarios of analytical work that I have performed. I should declop habits that ensure I am descriptive in my portfolio so when looking back at my projects I can cleary remember my workflow. I should also decelop habits to clearly write out code and include lots of informative notes so that if I don't use these skills consistently after completing this course, I am able to review the material in my portfolio as a reminder on how to perform certain analytical functions.
