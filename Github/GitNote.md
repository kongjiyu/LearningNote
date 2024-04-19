# Git Project Management Note
1. Clone repo
```cmd
git clone {link}
```

2. Open new branch
```cmd
git checkout -b {my-feature}
```

3. After change, check difference
```cmd
git diff
```

4. Add change file
```cmd
git add {changed_file}
```

5. commit changes
```cmd
git commit
```

6. Push branch
```cmd
git push origin {my-feature}
```

7. change to main branch
```cmd
git checkout main
```

8. pull main branch into git and disk
```cmd
git pull origin master
```

9. go back to branch
```cmd
git checkout {my-feature}
```

10. Take the latest main 
```cmd
git rebase main
```

11. force push branch 
```cmd
git push -f origin {my-feature}
```

12. Squash and merge branch

13. Delete branch at github

14. go back main branch
```cmd
git checkout main
```

15. Delete branch at git
```cmd
git branch -D {my-feature}
```

16. pull latest master from github
```cmd
git pull origin master
```