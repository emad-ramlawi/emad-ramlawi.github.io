### SVN code acess

ssh tech@192.168.103.21

```
sudo nano /etc/subversion/conf/svn_access_file
```

Add user to internal + workgroup (QA) using ktoole and eramlawi naming convention, and make password 

```
BACKUP the htpasswd file
cp /etc/subversion/passwd /etc/subversion/passwd.backup
cp /etc/subversion/passwd /home/eramlawi/
cat  /etc/subversion/passwd
sudo htpasswd /etc/subversion/passwd  sbozdag
```

Then:

```
sudo /etc/init.d/apache2 reload
```

