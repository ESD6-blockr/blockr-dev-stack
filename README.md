# DEV Stack
Docker-compose stack of all essential blockr modules

## Steps
 - Clone project
 - Run `git submodule init`
 - Run `git submodule update --remote`
 - Run `docker-compose up --build`
 
By default the submodules master is used. If you want to change to branch you can change the .gitsubmodule file and change the branch.
Make sure you don't push this branch change to this repo.
