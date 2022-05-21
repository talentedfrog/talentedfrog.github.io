# Jim's Blog HomePage

* Todo List

- [x] DPS Hardware spec compare
- [x] Finish a Pin Config with pin map & sch
- [x] Learn about the Hardware of tester
- [x] make a intern report
- [ ] a shmoo test based on lib func

* Login remote docker in local terminal by setting local port forwarding.

In remote docker

```bash
apt-get install openssh-server

vim /etc/ssh/sshd_config # edit Port & PermitRootLogin
service ssh restart

passwd # set Unix Root Passwd

ssh-keygen -t rsa -C "yourEmail"
```

In local terminal (Windows Terminal or Powershell)

```bash
ssh -L portB:HostC:portC user@HostC
```

* Solve remote docker git problems.


```bash
cd prj_path
rm -rf .git
git init
git remote add origin remote_repo_url
mv .git /home/new_name.git
ln -s /home/new_name.git .git
git fetch --all
git reset --hard origin/master
git branch --set-upstream-to=origin/master master
```

