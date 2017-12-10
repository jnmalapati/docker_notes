
#Swarm Mode Theory
~ new stuff in docker 1.12 and later....

# Terminology: 
A cluster = A swarm
Engines in a swarm run in swarm mode
It's all about true native clustering
<< a collection of docker engines joined into a cluster is a swarm>>

Manager nodes maintain the swarm
 ~ H/A - recommend 3 or 5
 ~ only one is leader

Services
 ~ Declarative & scalable
 
for e.g.,
docker service create --name web-fe --replicas 5 ...
   ~ makes 5 running
   
Tasks
 ~ Assigned to workers
 ~ containers
 
 #Building a Swarm
 
 6 - Nodes swarm
 
 3 x Managers
 3 X workers
 
 - docker swarm init --advertise-addr <ip>:<port> --listen-addr <sameip>:<sameport>
 

