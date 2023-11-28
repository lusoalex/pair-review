# Pair Review

This is an empty project used only for pair review exercices.

## How-to

1. You will need a GitHub account.
2. Fork https://github.com/lusoalex/pair-review
3. Code and create a pull-request once ready

### Create a pull-request within an existing code base

Replace place holders ${XXX} before running scripts.  
_Ex: if your current code is located to `~/dev/interview/exercice`, this will give:_
- ${SOURCE_CODE_ROOT_PATH_FOLDER} =>  _`~/dev/interview` (without the last trailing slash)_
- ${FOLDER_NAME} => _`exercice`_


``` BASH
# Go to your current source code folder.
cd ${SOURCE_CODE_ROOT_PATH_FOLDER}/${FOLDER_NAME}
rm -rf .git
cd ..
# Run below command by replacing ${GH-ACCOUNT} with your github account
git clone git@github.com:${YOUR-ACCOUNT}/pair-review.git
cp -r ${FOLDER_NAME}/* pair-review
cd pair-review
git add .
git commit -m "feat: exercice"
git branch -M feat/exercice
git push --set-upstream origin feat/exercice
# Use github.com web interface and create a pull-request
```