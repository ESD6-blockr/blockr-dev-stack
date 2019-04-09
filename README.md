# DEV Stack
Docker-compose stack of all essential blockr modules

## Steps run blockcahin for the first time
 - Clone project
 - Change .gitmodules branch of validator to `Develop`
 - Run `git submodule init`
 - Run `git submodule update --remote`
 - Run `docker-compose up --build`
 - Run `docker-compose exec validator_backup sh`
 - Run `cat /keys/.keys`
 - Copy `pubKey` and `privKey` to `PUBKEY_ADMIN` and `PRIVKEY_ADMIN` in `blockr-validator/src/.env`
 - Run `docker-compose down`
 - Run `docker-compose up --build`

# Steps run blockchain
  - Run `docker-compose up --build`
 
By default the submodules master is used. If you want to change to branch you can change the .gitsubmodule file and change the branch.
Make sure you don't push this branch change to this repo.
