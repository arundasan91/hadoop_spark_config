# Hadoop and Spark Configuration

### These files will serve as an easy to modify template for Hadoop and Spark Clusters.

Points to note:    
1. `xml` files are placed in `master` folder.    
2. Change `localhost` in `xml` files to respective node's (master of slave) hostname.    
3. Only for `core-site.xml` file, change `localhost` to name of the master node.

Easily change `localhost` to respective hostname using `sed` command.    
For example:    
```
sed -i "s|localhost|$HOSTNAME|g" mapred-site.xml
```
