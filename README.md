# Open Source CI/CD Pipeline

```
Current setup, running on AWS:

GitHub code changes automatically triggers 
 Jenkins builds artifact (Maven) 
   copies .war to Ansible/Docker server 
   Ansible-Playbook1 creates Docker image of tomcat and copies .war to /webapps > uploads it to DockerHub 
   Ansible-Playbook2 removes any running containers from the targets, pulls docker image from PB1, and runs the new containers

```


### Up Next:
- Kubernetes

