# Jim's Blog HomePage

* Todo List

- [x] DPS Hardware spec compare
- [x] Finish a Pin Config with pin map & sch
- [x] Learn about the Hardware of tester
- [x] make a intern report
- [ ] a shmoo test based on lib func

* Login remote docker in local terminal.


```bash
apt-get install openssh-server

vim /etc/ssh/sshd_config # edit Port & PermitRootLogin
service ssh restart

passwd # set Unix Passwd
```

install service

edit config to set port and login method

set root passwd

* Solve remote docker git problems.


```bash
cd prj_path
rm -rf .git
git remote add origin remote_repo_url
mv .git /home/new_name.git
ln /home/new_name.git .git
git fetch --all
git reset --hard origin/master
git branch --set-upstream-to=origin/master master
```

