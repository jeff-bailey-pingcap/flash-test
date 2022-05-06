Working example of setting up GitHub repositories and getting it to work with the PingCAP Flash environment.

# Flash Experimentation Notes

## Create a GitHub repository (CLI)
```
cd ~/git
mkdir flash-test
cd flash-test
touch README.md -- edit the file so there is something in it.
git init .
git branch -m master
git add .
git commit -m "initial commit"
```


Create a new Github repository (this will prompt for the password or Personal Access Token)
```
curl -u 'jeff-bailey-pingcap' https://api.github.com/user/repos -d '{"name":"flash-test","description":"This project is a Flash test"}'
git remote add origin git@github.com:jeff-bailey-pingcap/flash-test.git
git push -u origin master
```
Now, edit the README.md file and save the changes...
```
git add .
git commit -m "Edited README.md"
git push -u origin master
```
At this point, we have a Github respository and can push/pull. 

## Setup Flash

