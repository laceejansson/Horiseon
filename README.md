# Horiseon
Horiseon is a marketing site that meets accessibility standards


## Create New Repository @ https://github.com/new
	- name it something that describes the content of the repository
	- give it a repository description that describes the functionality of the repository

## Clone the repository
	- `cd ~/Desktop`
	- `git clone git@github.com:laceejansson/Horiseon.git`
	- `cd Horiseon`
	- `git status`

expected output: 

```
Lacees-MacBook-Pro:Horiseon laceejansson$ git status
On branch master
Your branch is up to date with 'origin/master'.
```


## Copy Website Content Into New Repository

We want to copy the same website that is contained within 01-HTML-Git-CSS/02-Homework/Develop/ into the root of our new repository.

    cp -r ../CLASS-CONTENT/Class-Content/01-HTML-Git-CSS/02-Homework/Develop/ ~/Desktop/Horiseon


## Create First Commit

### Verify your local changes are being picked up by git with git status

```
Lacees-MacBook-Pro:Horiseon laceejansson$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        assets/
        index.html
```

### Add files to staging with git add

    Lacees-MacBook-Pro:Horiseon laceejansson$ git add .

### Verify staged files with git status

```
Lacees-MacBook-Pro:Horiseon laceejansson$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   README.md
        new file:   assets/css/style.css
        new file:   assets/images/brand-awareness.png
        new file:   assets/images/cost-management.png
        new file:   assets/images/digital-marketing-meeting.jpg
        new file:   assets/images/lead-generation.png
        new file:   assets/images/online-reputation-management.jpg
        new file:   assets/images/search-engine-optimization.jpg
        new file:   assets/images/social-media-marketing.jpg
        new file:   index.html

```

### Commit changes

Formulate a short commit message to describe the changes you have made

```
Lacees-MacBook-Pro:Horiseon laceejansson$ git commit -m "copy the website to refactor into new repository"
[master a261de4] copy the website to refactor into new repository
 10 files changed, 352 insertions(+)
 create mode 100644 assets/css/style.css
 create mode 100644 assets/images/brand-awareness.png
 create mode 100644 assets/images/cost-management.png
 create mode 100644 assets/images/digital-marketing-meeting.jpg
 create mode 100644 assets/images/lead-generation.png
 create mode 100644 assets/images/online-reputation-management.jpg
 create mode 100644 assets/images/search-engine-optimization.jpg
 create mode 100644 assets/images/social-media-marketing.jpg
 create mode 100644 index.html

```

### Push local changes

    git push origin master


## Publish Website

Publish the website to the internet so that we can view our changes online as we push them to github.

Visit https://github.com/laceejansson/Horiseon/settings > Github Pages 

ensure that in the user interface:
branch = master
folder = root

click save then scroll back down to Github Pages to copy the new url.

    Your site is ready to be published at https://laceejansson.github.io/Horiseon/.



