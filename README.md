Deploy:

```
git clone https://github.com/imjorge/jenkins-on-flynn.git
cd jenkins-on-flynn
flynn create jenkins
git push flynn master
```

Grab the login token from the logs:

```
flynn log 
```

It looks something like `e7af1c1f1574b548febd50e1bafb90b`.

Go to http://jenkins.$CLUSTER_DOMAIN and enter the login token. Then configure Jenkins.

Bare in mind that, until Flynn gets permanent volumes, this is ephemeral.
