# this is the step by step walkthrough of this project

Open Terminal

Open text editor

Figure out where we will be saving files and navigate there in terminal

Terminal (T):
mkdir exceptional-realty (this makes a new folder called exceptional-realty)

Next we make the readme file

T:
touch README.md (touch = create README file in markdown format)

next lets create a git ignore file to prevent hidden files from getting into our git repository

T:
touch .gitignore
T:
subl . (opens folder in sublime editor)

Add contents to README.
title, description, contact info, etc.

In the .gitignore file, add the recommended list from https://github.com/github/gitignore
(we haven't covered the global .gitignore yet)

T:
ls -a (will show all files, including the usually hidden .gitignore)

Now it's time to create a new git repository

T:
git init  (initializes new empty repo)

T:
git add . (add all files in dir to repo)

T:
git commit -m "first commit" (commit to repo, add message)

Navigate to github, click upper right corner +, click new repository

Give github repo same name and description as project

Make it public and we already have a readme

T: 
git remote add origin git@github.com:iandevivi/exceptional-realty.git
(this is copied from the bottom of the github screen after creating repo)

typing git remote in T: will return "origin"

T:
git push -u origin master (-u sets up tracking between local and remote masters)

refreshing github should show the files synced to github

Now we want to start creating branches as we work on the project and add pages to it.

T:
git co -b main-pages (creates a repo branch called 'main-pages')

Let's start making html pages for our project.  First and foremost is index.html

T:
touch index.html (this must be named index.htm or index.html so the web protocols know what to look for first)

T:
touch contact.html
T:
touch market-report.html
T:
touch new-properties.html
T:
touch real-estate-listings.html

This creates all of these html documents in the exceptional-realty directory.
Names are important for search engines - name pages based on searchable terms.

We need an images folder.

T: 
mkdir images

Some unrelated bash info for copying files...

cd to file location you want to move.
T:
cp file-to-copy.jpg ~/dev/exceptional-realty/images/file-to-copy.jpg

--------------
Next learn lesson
--------------

Open index.html

all indexs start with declaring document type.

"<!DOCTYPE html>" does not require a closing

then we use the html element.  Add attribute in the opening tag to include a language.
<html lang="en"> iso 2 language code
two main sections of every webpage

head
- can't see on page, for browser and search engines, and title
body
- everything we can see.  images, texts, links, media

--------------
Next learn lesson
--------------






