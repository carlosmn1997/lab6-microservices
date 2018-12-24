* **The two microservices are running and registered (two terminals, logs screenshots).**

1. Microservice account service.
![Figure 1](images/terminalAccount.PNG "Terminal account service")
![Figure 2](images/webAccount.PNG "Web account service")
1. Microservice web service.
![Figure 1](images/terminalWeb.PNG "Terminal web service")
![Figure 2](images/webWeb.PNG "Web web service")

* **The service registration service has the two microservices registered (a third terminal, dashboard screenshots)**
In the figure bellow it can be seen the two instances of both microservices.
![Figure 1](images/registrationWeb.PNG "Registration of the instances")


* **A second account microservice is running in the port 4444 and it is registered (a fourth terminal, log screenshots).**
The new service can be run in 4444 changing the file [application.yml](accounts/src/main/resources/application.yml)
![Figure 1](images/2instances.PNG "Registration of the new instance")
![Figure 2](images/terminalAccount2.PNG "Terminal of the new instance in 4444 of account microservice")


* **A brief report describing what happens when you kill the microservice with port 2222. Can the web service provide information about the accounts? Why?**
When the microservice in with the port 2222 is stopped and then it's tried to get information about some of the example accounts, the microservice switch is provider to the server 4444. It can be seen in the figure bellow:
![Figure 1](images/newProvider.PNG "The provider has changed")