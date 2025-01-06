# Command line instructions
```
Git global setup
git config --global user.name "XXXX"
git config --global user.email "XXXX@YYY.com"
```

# Create a new repository
```
git clone https://git.huawei.com/securitydata/gitcommand.git
cd gitcommand
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master
```
# Existing folder
```
cd existing_folder
git init
git remote add origin https://git.huawei.com/securitydata/gitcommand.git
git add .
git commit -m "Initial commit"
git push -u origin master
```
# Existing Git repository
```
cd existing_repo
git remote rename origin old-origin
git remote add origin https://git.huawei.com/securitydata/gitcommand.git
git push -u origin --all
git push -u origin --tags
```
# FQA:
```
if there is an error about git push,
please run： git.exe pull --progress -v --no-rebase --allow-unrelated-histories "origin" master
```

# exception file .gitignore
like this sample
```
/files/
/service/record.txt
/config.json
```
