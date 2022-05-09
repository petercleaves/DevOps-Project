# Open Source CI/CD Pipeline
Example deployed docker container:
http://3.144.4.72:8080/webapp/
```
Current setup, running on AWS:

GitHub code changes automatically triggers 
 Jenkins builds hello-world java web artifact (Maven) 
   copies .war to Ansible/Docker server 
   Ansible-Playbook1 creates Docker image of tomcat and copies .war to /webapps > uploads it to DockerHub 
   Ansible-Playbook2 removes any running containers from the targets, pulls docker image from PB1, and runs the new containers

```


### Up Next:
- Kubernetes



