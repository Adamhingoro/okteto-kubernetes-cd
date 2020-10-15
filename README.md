# Okteto
Is a online service for developers to test the k8s applications on a test-envoriment. 
I really like the service it is free and you can easilly test and deploy your cloud-native applications. 
https://okteto.com/

# Travis with Okteto. 
Travis CI/CD is good and we can use kubectl to push the new changes to the cluster.

# Okteto Kubernetes CI/CD
What we did here is simple. 

we simply base64 encoded the `okteto-kube.config` file and stored it in `travis-secrets`. 
instead of passing the file in the repo we did it by passing it to travis. 

now on the build it will decode the base64 content. 
set the **KUBECONFIG** variable

and you are ready to do your kubectl updates. 

Thank you. 
