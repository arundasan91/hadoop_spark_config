# Hadoop and Spark Configuration

### These files will serve as an easy to modify template for Hadoop and Spark Clusters.

Points to note:    
1. `xml` files are placed in `master` folder.    
2. Change `localhost` in `xml` files to respective master node's hostname.    

Easily change `localhost` to respective hostname using `sed` command.    
For example in master node:    
```
sed -i "s|localhost|$HOSTNAME|g" mapred-site.xml
```
In slave nodes, 
```
sed -i "s|localhost|__hostname_of_master_node__|g" mapred-site.xml
```
