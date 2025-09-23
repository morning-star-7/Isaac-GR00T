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



# conect to gpu in jupyter notrbook
1. srun --account cortex -q cortex_high --nodes=1 --ntasks-per-node=1 --gpus-per-node=1 --cpus-per-task=12 --mem=1024G --time-min=900 --pty /bin/bash
2. conda activate gr00t
2. jupyter notebook --port 8899 --ip 0.0.0.0
3. Now open your IPYNB in vscode and click on "Select kernel". Choose "Existing Jupyter server"
4. http://a100-st-p4de24xlarge-3:8899/tree?token=1fac94be9a94dc11151ca4998148bc5c402f2fa3e7b8e18c