# kube-app-vprofile

 https://www.udemy.com/course/decodingdevops/

 Credits: Iram

### Stack technologies
For this project

![Alt text](image.png)
---
1. ** Encode secrets **

`
echo -n "password" | base64
`
    
2. Config NFS server

make sure you have the correct configuration on your nfs server
```
/srvnfs/kubernetes x.x.x.x(rw,sync,no_subtree_check,no_root_squash)

chown -R nobody:nogroup /srvnfs/kubernetes/ 

service nfs-kernel-server reload 
```

3. Deploy all definition files

` kubectl create -f . `