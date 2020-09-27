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

### Verify your local changes are being picked up by git

```
Lacees-MacBook-Pro:Horiseon laceejansson$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        assets/
        index.html
```

### Add files to staging

    Lacees-MacBook-Pro:Horiseon laceejansson$ git add .

### Verify staging

```
Lacees-MacBook-Pro:Horiseon laceejansson$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

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

