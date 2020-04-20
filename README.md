# Okteto Kubernetes CI/CD
What we did here is simple. 

we simply base64 encoded the `okteto-kube.config` file and stored it in `travis-secrets`. 
instead of passing the file in the repo we did it by passing it to travis. 

now on the build it will decode the base64 content. 
set the **KUBECONFIG** variable

and you are ready to do your kubectl updates. 

Thank you. 