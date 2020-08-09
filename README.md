## Manual Steps to Install MongoDB 

1. Set the repo 

```
# cat /etc/yum.repos.d/mongodb-org-4.2.repo
[mongodb-org-4.2]
name=MongoDB Repository
baseurl=https://repo.mongodb.org/yum/redhat/$releasever/mongodb-org/4.2/x86_64/
gpgcheck=1
enabled=1
gpgkey=https://www.mongodb.org/static/pgp/server-4.2.asc
```


2. Install MongoDB 

```
# yum install -y mongodb-org
```

3. Start the Service 

```
# systemctl enable mongod
# systemctl start mongod 
```

4. Load MongoDB for the application.

Clone the MongoDB Repository.

```bash
cd mongodb 
mongo <catalogue.js 
mongo <users.js
```


