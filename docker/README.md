## Container and Docker

Before we start reviewing Docker, we need to take a look at the concept of Infrastructure as a service (IaaS), Platform as a service (PaaS) and Software as a service (SaaS) as docker belongs to PaaS category. Also, we review the history of containers.

### Infrastructure as a service (IaaS)

    TIaaS, is a step away from on-premises infrastructure. It’s a pay-as-you-go service where a third party provides you with infrastructure services, like storage and virtualization, as you need them, via a cloud, through the internet. 

    As the user, you are responsible for the operating system and any data, applications, middleware, and runtimes, but a provider gives you access to, and management of, the network, servers, virtualization, and storage you need. 

### Platform as a service (PaaS)

    PaaS is another step further from full, on-premise infrastructure management. It is where a provider hosts the hardware and software on its own infrastructure and delivers this platform to the user as an integrated solution, solution stack, or service through an internet connection.

    Primarily useful for developers and programmers, PaaS allows the user to develop, run, and manage their own apps without having to build and maintain the infrastructure or platform usually associated with the process. 


### Software as a service (SaaS)
    SaaS, also known as cloud application services, is the most comprehensive form of cloud computing services, delivering an entire application that is managed by a provider, via a web browser. 

    Software updates, bug fixes, and general software maintenance are handled by the provider and the user connects to the app via a dashboard or API. There’s no installation of the software on individual machines and group access to the program is smoother and more reliable. 

![IaaS,PaaS and SaaS](https://www.redhat.com/cms/managed-files/iaas-paas-saas-diagram5.1-1638x1046.png)

### History of Containers
* 1979: Unix V7
* 2000: FreeBSD Jails
* 2004: Solaris Containers
* 2005: Open VZ (Open Virtuzzo)
* 2006: Process Containers
* 2008: LXC
* 2011: Warden
* 2013: LMCTFY
* 2013: Docker
* 2016: The Importance of Container Security Is Revealed
* 2017: Container Tools Become Mature

Docker is a set of platform as a service (PaaS) products that use OS-level virtualization to deliver software in packages called containers. Containers are isolated from one another and bundle their own software, libraries and configuration files; they can communicate with each other through well-defined channels. All containers are run by a single operating system kernel and therefore use fewer resources than virtual machines.

## More Contents
### To read

### To watch

### Cheat Sheets
1. [Docker Cheat Sheet](https://www.docker.com/sites/default/files/d8/2019-09/docker-cheat-sheet.pdf)
2. [The Ultimate Docker Cheat Sheet](https://dockerlabs.collabnix.com/docker/cheatsheet/)