# env_fix

The first line is to go through each commit history and remove everything that has a .env
`git filter-branch --tree-filter 'rm -f .env' HEAD` 

2nd line is forcefully pushing these changes to github.com
`git push origin --force --all` 

3rd line is optional if you used any tags. This will also force the changes to the tags commit. 
`git push origin --force --tags`
