# Jim's Blog HomePage

* Login remote docker in local terminal.
```bash
apt-get install openssh-server

vim /etc/ssh/sshd_config
/etc/init.d/ssh restart

passwd
```
> install service
> edit config to set port and login method
> set root passwd

* Solve remote docker git problems.
* 
```bash
cd prj_path
rm -rf .git
git remote add origin remote_repo_url
git pull
mv .git /home/new_name.git
ln /home/new_name.git .git
git fetch --all
git reset --hard origin/master
git branch --set-upstream-to=origin/master master
```

