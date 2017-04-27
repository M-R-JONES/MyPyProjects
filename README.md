# MyPyProjects
An open repository in which I'll dabble with various Pythonic things.



## Ignoring PyCharm workspace:
- remove the .idea directory from git cache (information from stackoverflow user amerdidit) http://stackoverflow.com/questions/19973506/cannot-ignore-idea-workspace-xml-keeps-popping-up 
1. mv .idea ../.idea_backup
2. rm .idea # in case you forgot to close your IDE
3. git add .idea 
4. git commit -m "Remove .idea from repo"
5. mv ../.idea_backup .idea

- Following is from (from user SomeAnonymousPerson on stackoverflow)

6. Generate git.txt file
7. Open command line and type "rename git.txt .gitignore"
8. Open .gitignore and add ".idea/workspace.xml" to the file and save
9. Ensure that .gitignore is placed in the working directory (not in the .git subdirectory)
10. Open the terminal/cmd in your working directory
11. Type the following 
12.	git rm -r --cached .
13.	git add .
14.	git commit -m ".gitignore is now working"
15.	git push
16.	git status #check if everything is up to date

