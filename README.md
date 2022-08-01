# ocp-RBAC

```
echo "# ocp-RBAC" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/alpha-wolf-jin/ocp-RBAC.git
git config --global credential.helper 'cache --timeout 7200'
git push -u origin main

git add . ; git commit -a -m "update README" ; git push -u origin main
```

**OCP environemnt**
```
$ oc get clusterversion
NAME      VERSION   AVAILABLE   PROGRESSING   SINCE   STATUS
version   4.10.11   True        False         47h     Cluster version is 4.10.11

$ oc get node
NAME                        STATUS   ROLES    AGE    VERSION
aro-pcnpf-master-0          Ready    master   2d1h   v1.23.5+9ce5071
aro-pcnpf-master-1          Ready    master   2d1h   v1.23.5+9ce5071
aro-pcnpf-master-2          Ready    master   2d1h   v1.23.5+9ce5071
aro-pcnpf-worker-eastus-1   Ready    worker   47h    v1.23.5+9ce5071
aro-pcnpf-worker-eastus-2   Ready    worker   47h    v1.23.5+9ce5071
aro-pcnpf-worker-eastus-3   Ready    worker   47h    v1.23.5+9ce5071

```

# Create htpasswd Authentication

```
$ sudo yum provides "*/htpasswd"
httpd-tools-2.4.37-47.module+el8.6.0+15654+427eba2e.2.x86_64 : Tools for use with the Apache HTTP Server
Repo        : rhel-8-for-x86_64-appstream-eus-rhui-rpms
Matched from:
Filename    : /usr/bin/htpasswd

$ sudo yum install httpd-tools -y


```
