# Aws

# what is AWS?
  
  1. stands for "Amazon web services".
  2. It is a cloud infrastructure where we can host our application.
  3. In 2006,Aws started to offer It services to the market in the form of webservices which is now a days known as Cloud Computing.

   Cloud Computing
     1. It is just a tern refer to storing and accessing the data over the internet.
     2. It doesnot store any data in the harddisk of your personal computer.
     3.  we can directly access data from remote server.

#Why Aws?

Hosting any web application
  1. purchase a server.
  2. if there is any database integrationthen purchase DB.
  3. Install JDK for java and differnt for different language.
  4. Setup complete infrastructure to host an application.

# problems
  
  1. If the user accessing or not accessing the application, we need to pay for it because of the purchase of server.
  2. It load is increase , we need to scale or increase the server to balance the load.

# Solution

  1. Aws provide to create a virtual machine. Inside this VM ,we can add a server a DB etc. (Multiple cloud infrastructure we can  build).
  2. In this cloud we donot need to plan for server and other IT infrastructure which take much time.
  3. we can easily scale the infrastructure.
  4. In Aws term this VM  is called EC2 instance (Elastic compute cloud).  
                   
# Create Account 

  1. Aws amazon.com
  2. create an account

# EC2 instance (A Virtual machine)

  1. Aws console
  2. service section
  3. compute > EC2 > launch instance
  4. choose Amazon machine image AMI (free tier eligible)
  5. instance type (free tier eligible)
  6. No. of instance
  7. add storage (8gb3)
  8. add tags
  9. configure security group type: custom TCP port: 8080 Source type: Anywhere
  10. key pair Download and save for further use
  11. launch
  12. click on file name
  13. edit name of instance
  14. click connect key and now we see all details about our instance

# how to deploy Spring boot project in aws using EC2

## Steps:

1. create a spring boot project with end point
2. add  <finalName>jarName </finalName> in pom.xml
    the jar will be generrated in target folder with jarName
3. strat the EC2 instance
    In Uduntu:
4.  copy the ssh url and paste it in terminal where the project path

# s3 

 main purpose is to store the jar/war file

# Create bucket

 1. Name the bucket and create
 2. make the bucket public otherwise,  it will show the error 403 forbidden
    To make the s3 bucket public
    1. select the bucket
    2. Actions > make it public using ACL
 3. now copy the IPv4 object url ans paste it in taht instance conncted terminalwith (wget + url)
 4. It start downloading
 5. when downloaded run by using command (java -jar jarname.jar)

# To run 

1. to get the base url  (EC2 > public DNS IPv4 url)
2. Then base url:port/endpoint wull how the result in browser
   

    
 

   
