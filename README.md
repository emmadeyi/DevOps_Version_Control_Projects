# DevOps_Version_Control_Projects
Project #1 for DevOps Journey

Objective: Learn Git basics and GitHub workflow.
Tasks and Implementation:
1.	Create a repository on GitHub:
o	Scenario: You decide to create a GitHub repository named personal-blog.
o	Action: Go to GitHub, click on the "New" button, and create a repository called personal-blog.
2.	Clone the repository locally:
o	Scenario: You want to start working on your blog website on your local machine.
o	Action: Open your terminal and clone the repository using the command:

```
git clone https://github.com/your-username/personal-blog.git
```
3.	Make several commits with meaningful messages:
o	Scenario: You begin by setting up the basic structure of your website, such as creating HTML, CSS, and JavaScript files.
o	Action:
```
git add index.html
git commit -m "Add initial HTML structure"
```
```
git add styles.css
git commit -m "Add CSS for homepage layout"

git add script.js
git commit -m "Add JavaScript for interactive features"
```
4.	Create and merge branches:
o	Scenario: You want to add a new feature to your blog, such as a contact form, without affecting the main branch.
o	Action:
```
git checkout -b feature-contact-form
# Add contact form code
git add contact.html
git commit -m "Add contact form page"

git checkout main
git merge feature-contact-form
```
5.	Resolve merge conflicts:
o	Scenario: While merging another branch, you encounter a merge conflict in styles.css.
o	Action:
```
git checkout -b feature-responsive-design
# Make changes to styles.css for responsive design
git add styles.css
git commit -m "Make site responsive"

git checkout main
git merge feature-responsive-design
# Resolve conflicts in styles.css manually
git add styles.css
git commit -m "Resolve merge conflict in styles.css"
```
6.	Push the merged changes to the repository:
o	Scenario: After merging your feature branches into the main branch, you want to update the remote repository with the latest changes.
o	Action:
```
git push origin main
```