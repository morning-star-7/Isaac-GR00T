# submodule
at :~/eai/robot_world_models folder
git submodule add https://github.com/morning-star-7/Isaac-GR00T.git projects/Isaac-GR00T
git add .gitmodules projects/Isaac-GR00T
git commit -m "add gr00t as submodule"
git push

# change http to git
git remote set-url origin git@github-morningstar7:morning-star-7/Isaac-GR00T.git


# push to submodule
- go the submodule folder
- commit
- git push

# uddate the main project
- cd /robot_world_models
- git add projects/Isaac-GR00T
- git commit -m "update groot submodule to latest commit"
- git push
