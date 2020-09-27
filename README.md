# Horiseon

Horiseon is a marketing site that meets accessibility standards

    git clone git@github.com:laceejansson/Horiseon.git

    https://laceejansson.github.io/Horiseon/

- [Horiseon](#horiseon)
  - [User Story](#user-story)
  - [Acceptance Criteria](#acceptance-criteria)
  - [Create New Repository @ https://github.com/new](#create-new-repository--httpsgithubcomnew)
  - [Clone the repository](#clone-the-repository)
  - [Copy Website Content Into New Repository](#copy-website-content-into-new-repository)
  - [Create First Commit](#create-first-commit)
    - [Verify your local changes are being picked up by git with git status](#verify-your-local-changes-are-being-picked-up-by-git-with-git-status)
    - [Add files to staging with git add](#add-files-to-staging-with-git-add)
    - [Verify staged files with git status](#verify-staged-files-with-git-status)
    - [Commit changes](#commit-changes)
    - [Push local changes](#push-local-changes)
  - [Publish Website](#publish-website)
  - [Refactor](#refactor)
    - [Change page title](#change-page-title)
    - [Use nav tag as semantic element](#use-nav-tag-as-semantic-element)
    - [Use footer tag as semantic element](#use-footer-tag-as-semantic-element)
    - [Fix nav bar header tag](#fix-nav-bar-header-tag)


## User Story

AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines

## Acceptance Criteria

GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title

## Create New Repository @ https://github.com/new

- name it something that describes the content of the repository
- give it a repository description that describes the functionality of the repository

## Clone the repository
- `cd ~/Desktop`
- `git clone git@github.com:laceejansson/Horiseon.git`
- `cd Horiseon`
- `git status`

- expected output: 

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

## Refactor

### Change page title

from

    <title>website</title>

to

    <title>Horiseon</title>

within the page head tag


### Use nav tag as semantic element

from

    <div class="header">

to

    <nav class="header">

within the page body tag


### Use footer tag as semantic element

from

    <div class="footer">

to

    <footer class="footer">

as the last tag in the body

### Fix nav bar header tag

from

    <h1>Hori<span class="seo">seo</span>n</h1>

to

    <h1>Horiseon</h1>

within the nav bar
