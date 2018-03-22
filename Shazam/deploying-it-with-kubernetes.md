# Step Two Deploying it with Kubernetes

Running Docker images is just great experience. Now I am ready to deploy the application to the IBM Cloud.

Before you begin, you must have a Pay-As-You-Go or Subscription IBM Cloud [http://bluemix.net](http://bluemix.net/)account to create a free cluster.

####To create a free Kubernetes cluster

>a. From the IBM Cloud Catalog go to Containers category, click Containers in Kubernetes Clusters.

>b. Read up on clusters, then click Create. Enter a Cluster Name.

>c. The default cluster type is free. Next time, you can create a standard cluster and define additional customizations, like the number of worker nodes.

>d. Click Create Cluster. The details for the cluster open, but the worker node in the cluster takes a few minutes to provision. You can see the status of the worker node in the Worker nodes tab. When the status reaches Ready, your worker node is ready to be used.

To set up the cluster took some time \(well you might look in the step three\). When it was done — my cluster was ready.

The really easy for the Kubernetes beginners way is to use the GUI provided by IBM Cloud. If you click on the name of your cluster you will be shown the next page with its details. Just follow directions to open the dashboard the item “Access” on your menu on the left as shown here:

####When everything is ready — you might open the dashboard.

You would need the Token for that:
```code
$ kubectl config view -o jsonpath=’{.users\[0\].user.auth-provider.config.id-token}’
```
```code
$ kubectl proxy
```

####Copy the token, and use it in the login screen.

I needed to create mysql-pod, mysql-service, and openliberty-pod \(the most atomic elements in the Kubernetes are “pods”\).

I simply clicked the create button and provided link to those 3 files in the following order:

>a. shazam4pets-mysql-pod.yaml

>b. shazam4pets-mysql-service.yaml

>c. shazam4pets-openliberty-rc.yaml

####Adding the YAML files.

![](https://cdn-images-1.medium.com/max/1600/1*3ta1th4DTx1R8RKoy-TNsQ.png)

The files were using the Docker images we created earlier. Their listings \(WATCH OUT SPACES ARE IMPORTANT — seriously 🥇\) comes in my repo

>a. shazam4pets-mysql-pod.yaml

>b. shazam4pets-mysql-service.yaml

We are ready to access it from our new UX. More details on the previous two steps are in my GitHub repo: [https://github.com/blumareks/2018-petstore](https://github.com/blumareks/2018-petstore)



