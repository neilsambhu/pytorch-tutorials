# PyTorch Tutorials
12/10/2023 8:59 PM: change remote
```
(pytorch_tutorials) nsambhu@CSE001022:~/github/pytorch_tutorials/tutorials$ git remote -v 
origin	git@github.com:pytorch/tutorials.git (fetch)
origin	git@github.com:pytorch/tutorials.git (push)
```
```
git remote set-url origin git@github.com:neilsambhu/pytorch_tutorials.git
```
No need to set upstream remote to `git@github.com:pytorch/tutorials.git` because I don't anticipate any updates.  
12/10/2023 9:07 PM: install requirements.  
```
pip install -r requirements.txt
```
12/10/2023 9:15 PM: I need to install Python 3.9
```
(pytorch_tutorials) nsambhu@CSE001022:~/github/pytorch_tutorials/tutorials$ pip install -r requirements.txt
ERROR: Ignored the following versions that require a different python version: 0.1.0.dev0 Requires-Python >=3.8; 0.1.0.dev1 Requires-Python >=3.8; 0.15.0 Requires-Python >=3.8; 0.5.0 Requires-Python >=3.8; 0.6.0 Requires-Python >=3.8; 0.6.1 Requires-Python >=3.8; 0.7.0 Requires-Python >=3.8; 0.7.1 Requires-Python >=3.8; 1.22.0 Requires-Python >=3.8; 1.22.1 Requires-Python >=3.8; 1.22.2 Requires-Python >=3.8; 1.22.3 Requires-Python >=3.8; 1.22.4 Requires-Python >=3.8; 1.23.0 Requires-Python >=3.8; 1.23.0rc1 Requires-Python >=3.8; 1.23.0rc2 Requires-Python >=3.8; 1.23.0rc3 Requires-Python >=3.8; 1.23.1 Requires-Python >=3.8; 1.23.2 Requires-Python >=3.8; 1.23.3 Requires-Python >=3.8; 1.23.4 Requires-Python >=3.8; 1.23.5 Requires-Python >=3.8; 1.24.0 Requires-Python >=3.8; 1.24.0rc1 Requires-Python >=3.8; 1.24.0rc2 Requires-Python >=3.8; 1.24.1 Requires-Python >=3.8; 1.24.2 Requires-Python >=3.8; 1.24.3 Requires-Python >=3.8; 1.24.4 Requires-Python >=3.8; 1.25.0 Requires-Python >=3.9; 1.25.0rc1 Requires-Python >=3.9; 1.25.1 Requires-Python >=3.9; 1.25.2 Requires-Python >=3.9; 1.26.0 Requires-Python <3.13,>=3.9; 1.26.0b1 Requires-Python <3.13,>=3.9; 1.26.0rc1 Requires-Python <3.13,>=3.9; 1.26.1 Requires-Python <3.13,>=3.9; 1.26.2 Requires-Python >=3.9; 2.0.0 Requires-Python >=3.8; 2.0.0rc0 Requires-Python >=3.8; 2.0.1 Requires-Python >=3.8; 2.0.1.post0 Requires-Python >=3.8; 2.0.2 Requires-Python >=3.8; 2.0.3 Requires-Python >=3.8; 2.0.4 Requires-Python >=3.8; 2.0.5 Requires-Python >=3.8; 2.0.6 Requires-Python >=3.8; 2.0.7 Requires-Python >=3.8; 2.0.8 Requires-Python >=3.8; 2.0.9 Requires-Python >=3.8; 2.0.9.post0 Requires-Python >=3.8; 2.1.0 Requires-Python >=3.8; 2.1.0rc0 Requires-Python >=3.8; 2.1.0rc1 Requires-Python >=3.8; 2.1.1 Requires-Python >=3.8; 2.1.2 Requires-Python >=3.8; 2.12.0 Requires-Python >=3.8; 2.12.1 Requires-Python >=3.8; 2.12.2 Requires-Python >=3.8; 2.12.3 Requires-Python >=3.8; 2.13.0 Requires-Python >=3.8; 2.14.0 Requires-Python >=3.8; 2.14.1 Requires-Python >=3.9; 2.15.0 Requires-Python >=3.9; 2.15.1 Requires-Python >=3.9; 2.3.0 Requires-Python >=3.8; 2.3.1 Requires-Python >=3.8; 2.3.2 Requires-Python >=3.8; 2.3.3 Requires-Python >=3.8; 2.7 Requires-Python >=3.8; 2.7.1 Requires-Python >=3.8; 2.7rc1 Requires-Python >=3.8; 2.8 Requires-Python >=3.8; 2.8.1 Requires-Python >=3.8; 2.8.1rc1 Requires-Python >=3.8; 2.8.2 Requires-Python >=3.8; 2.8.3 Requires-Python >=3.8; 2.8.4 Requires-Python >=3.8; 2.8.5 Requires-Python >=3.8; 2.8.6 Requires-Python >=3.8; 2.8.7 Requires-Python >=3.8; 2.8.8 Requires-Python >=3.8; 2.8rc1 Requires-Python >=3.8; 3.0 Requires-Python >=3.8; 3.0.0 Requires-Python >=3.8; 3.0b1 Requires-Python >=3.8; 3.0rc1 Requires-Python >=3.8; 3.1 Requires-Python >=3.8; 3.1rc0 Requires-Python >=3.8; 3.2 Requires-Python >=3.9; 3.2.1 Requires-Python >=3.9; 3.2rc0 Requires-Python >=3.9; 3.6.0 Requires-Python >=3.8; 3.6.0rc1 Requires-Python >=3.8; 3.6.0rc2 Requires-Python >=3.8; 3.6.1 Requires-Python >=3.8; 3.6.2 Requires-Python >=3.8; 3.6.3 Requires-Python >=3.8; 3.7.0 Requires-Python >=3.8; 3.7.0rc1 Requires-Python >=3.8; 3.7.1 Requires-Python >=3.8; 3.7.2 Requires-Python >=3.8; 3.7.3 Requires-Python >=3.8; 3.7.4 Requires-Python >=3.8; 3.8.0 Requires-Python >=3.9; 3.8.0rc1 Requires-Python >=3.9; 3.8.1 Requires-Python >=3.9; 3.8.2 Requires-Python >=3.9; 4.0.0.dev1 Requires-Python >=3.8; 6.0.0 Requires-Python >=3.8; 6.0.0b1 Requires-Python >=3.8; 6.0.0b2 Requires-Python >=3.8; 6.0.1 Requires-Python >=3.8; 6.1.0 Requires-Python >=3.8; 6.1.1 Requires-Python >=3.8; 6.1.2 Requires-Python >=3.8; 6.1.3 Requires-Python >=3.8; 6.2.0 Requires-Python >=3.8; 6.2.1 Requires-Python >=3.8; 7.0.0 Requires-Python >=3.8; 7.0.0rc1 Requires-Python >=3.8; 7.0.1 Requires-Python >=3.8; 7.1.0 Requires-Python >=3.8; 7.1.1 Requires-Python >=3.8; 7.1.2 Requires-Python >=3.8; 7.2.0 Requires-Python >=3.9; 7.2.1 Requires-Python >=3.9; 7.2.2 Requires-Python >=3.9; 7.2.3 Requires-Python >=3.9; 7.2.4 Requires-Python >=3.9; 7.2.5 Requires-Python >=3.9; 7.2.6 Requires-Python >=3.9
ERROR: Could not find a version that satisfies the requirement torchrl==0.2.1 (from versions: 0.0.1a0, 0.0.1b0, 0.0.1rc0, 0.0.2a0, 0.0.3, 0.0.4a0, 0.0.4b0, 0.0.4, 0.0.5, 0.1.0, 0.1.1)
ERROR: No matching distribution found for torchrl==0.2.1
```
12/10/2023 9:41 PM: requirements are complete.  
12/10/2023 9:56 PM: command to run works.  
```
(pytorch_tutorials) nsambhu@CSE001022:~/github/pytorch_tutorials/tutorials$ python intermediate_source/reinforcement_q_learning.py 
```
