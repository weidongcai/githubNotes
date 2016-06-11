# in Linux
# configure git for the first time
git config --global user.name "yourgithubuserid"
git config --global user.email "youremail"

# generate a local key
cd ~
cd .ssh
ssh-keygen -t rsa -C "youremail"

# check generated key
ls ~/.ssh/id_rsa
ls ~/.ssh/id_rsa.pub

# run ssh agent in background
ssh-agent -s

# 
ssh -T git@github.com
