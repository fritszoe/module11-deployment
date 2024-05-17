## Hello Minikube  
1. Compare the application logs before and after you exposed it as a Service.  
    Yes, The service can receive requests so that the log will record requests that have been made, it adds every time the page is refreshed.  
    ![](image1.png)  
2. Notice that there are two versions of `kubectl get` invocation during this tutorial section. The first does not have any option, while the latter has `-n` option with value set to `kube-system`.  
    By using -n, we state that the service we want is from the namespace. This is needed if for example there are many different services that have the same name and are spread across many namespaces.