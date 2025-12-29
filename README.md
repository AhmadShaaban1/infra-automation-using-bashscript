  # VagrantProject
Vagrant Multi-VM Setup for Web Application This Vagrantfile sets up a multi-VM environment for a web application with different components such as a database server, memcached server, RabbitMQ server, application server (Tomcat), and a web server (Nginx). Each VM is provisioned with the necessary software using shell scripts


![image](https://github.com/user-attachments/assets/a0122911-9939-4531-964a-defa2fc9f2c5)


# What tools will we use in the project?

# Prerequisite
1. Oracle VM Virtualbox
2. Vagrant                                                                                                
3. Vagrant plugins

# PROVISIONING
Services
1. Nginx => Web Service
2. Tomcat => Application Server                                                                            

3. RabbitMQ => Broker/Queuing Agent
4. Memcache => DB Caching
5. ElasticSearch => Indexing/Search service
6. MySQL => SQL Database 

![image](https://github.com/user-attachments/assets/a4031b02-40c4-4d91-9aad-7565d6d3ac7d)

# Project Steps

# 1:Create shell script (Backend vms ) 
 Create a ShellScript file for Database we will call mariadb.sh  We will write the following in the file 

![image](https://github.com/user-attachments/assets/069d7a26-b769-438d-a0bb-0daa7c5f0aa0)

![image](https://github.com/user-attachments/assets/f13facf4-6784-459f-8f16-6250e91e57f4)

![image](https://github.com/user-attachments/assets/9106d02b-b5c5-46ac-a797-a3aabd6c6391)


#2 Create a ShellScript file for Memcached we will call memcashed.sh  We will write the following in the file 

  ![image](https://github.com/user-attachments/assets/3c3e5102-c23b-4334-b893-befa45773ace)


#3 Create a ShellScript file for RabbitMQ  we will call rabbitmq.sh  We will write the following in the file 

![image](https://github.com/user-attachments/assets/14c2deae-c910-453c-a3b2-a8fa088a9233)


#4 Create a ShellScript file for APP in clude ( tomcat , nginx )

# 1: TOMCAT

![image](https://github.com/user-attachments/assets/79fab7ca-679c-42e2-973d-155aa85eb74c)


![image](https://github.com/user-attachments/assets/ec062160-3fc3-4818-a280-a3163d61a173)


![image](https://github.com/user-attachments/assets/ae812301-50e4-4518-b4e9-c0fd00b13d91)


![image](https://github.com/user-attachments/assets/3375b7f6-78c0-45dd-8cde-2424b0b2692c)

# 2: NGINX 
![image](https://github.com/user-attachments/assets/45b333b8-8934-44c8-907e-bdd324c177a4)

# After writing the scripts
 we will write a vagrantfile, which should be like this, and we will put in it all the VM that we will create, and we will also make a private network and connect the VM to each other and introduce them 

 ![image](https://github.com/user-attachments/assets/31f873bf-9913-43f4-b71d-a03b8ede2cb9)

 
 ![image](https://github.com/user-attachments/assets/8af07c38-6f23-4e41-99c1-793ecde28ff2)

 ![image](https://github.com/user-attachments/assets/c59ee219-e8b8-4573-a174-2bf8496ef1ca)

 # After all these steps, type inside the cmd in its own path 


 And in the end this is the picture of the project 

![image](https://github.com/user-attachments/assets/d0e29e05-a444-4c23-9757-c3f63a38e0d8)





 


 








