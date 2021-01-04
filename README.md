# wordpress_using_k8s
Here in this repo i have deployed wordpress using k8s manifests

used kustomization method to deploy wordpress 
But u can use various method like manifests of configmap, by kubectl method or by kustomization method 
A Secret is an object that stores a piece of sensitive data like a password or key. Since 1.14, kubectl supports the management of Kubernetes objects using a kustomization file. You can create a Secret by generators in kustomization.yaml.

Add a Secret generator in kustomization.yaml from the following command. You will need to replace YOUR_PASSWORD with the password you want to use.

Add resource configs for MySQL and WordPress
The following manifest describes a single-instance MySQL Deployment. The MySQL container mounts the PersistentVolume at /var/lib/mysql. The MYSQL_ROOT_PASSWORD environment variable sets the database password from the Secret.

use wordpress db host as wordpress db name and password as passed by secrets
