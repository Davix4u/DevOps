# DOCKERFILE 

Docker can build images automatically by reading the instructions from a Dockerfile. A Dockerfile is a text document that contains 
all the commands a user could call on the command line to assemble an image. This page describes the commands you can use in a Dockerfile.

 For this project will be using Docker Images 

 ### Step 1  Create a Directory and a dockerfile
 We need to creat a New working directory on our linux machine 

 sudo mkdir Project 
 cd Project

 <img width="921" alt="CD project" src="https://github.com/Davix4u/DevOps/assets/130823585/1a050abe-f344-4af7-87f4-0e66b81e9db1">

 Inside the project directory , create a file call dockerfile with this command
 sudo nano dockerfile  
write this in the file 
" FROM nginx:latest
  COPY ./index.html  /usr/share/nginx/html

  <img width="921" alt="nano dockerfile" src="https://github.com/Davix4u/DevOps/assets/130823585/ce861372-05a7-4829-ae78-c2e4e2e07520">

. MEANS current Working directory
/ MEANS  look for the file index.html
COPY MEANS to over write the content in Nginx in /usr/share/nginx/html

### STEP 2 Creat a index.html file
Create a file in the same project directory called  index.html
sudo nano index.html 

<img width="927" alt="nano index html" src="https://github.com/Davix4u/DevOps/assets/130823585/3a64bdf5-4620-45c3-981b-8e00e5a7a6cc">

you can write this in the file created

<img width="923" alt="index htm" src="https://github.com/Davix4u/DevOps/assets/130823585/a3804594-5f69-4e4c-a1de-0560edfebf74">

### step 3 
we use our docker build command , remember we dont need to memorise the command . The idea of every tools is to know , how it works 
we should first try this command 

docker build --help  ( to get the next syntax to use )

<img width="918" alt="dcoker-build --help" src="https://github.com/Davix4u/DevOps/assets/130823585/5554fc55-1dc6-41ad-8aa7-430175c1ae60">

Build Image 
docker build -t cg-app. 

<img width="914" alt="Docker build " src="https://github.com/Davix4u/DevOps/assets/130823585/21f5feea-6fe0-4c8d-8fea-f64b99e51a41">

let me explain the syntax
-t MEANS tags = cg-app:v1
. MEANS docker file is in the working directory 
NOTE: the dot (.) is a very important syntax

### step 4  Run images
 docker run --help  

 <img width="880" alt="docker run --help" src="https://github.com/Davix4u/DevOps/assets/130823585/5b4881ec-9f25-44a2-9883-afcc4bdf7363">

run our images with this  command 
docker run -d -p 80:80 --name webpage-html cg-app

<img width="920" alt="docker run html" src="https://github.com/Davix4u/DevOps/assets/130823585/a3bdcc7e-1e4c-4115-9ef5-5591e93bfded">

let's explain the syntax
-d = detach mode -p = port --name = name giving to the website,  Port:8080 is always open on our localhost

to confirm if it was a success, run the following command 
curl -v localhost80

<img width="677" alt="curl-host" src="https://github.com/Davix4u/DevOps/assets/130823585/f6ccfcac-5b3b-48e9-945e-2829aec2fa1c">

go to the localhost on your computer: localhost:8080

<img width="822" alt="docker-loaclhost" src="https://github.com/Davix4u/DevOps/assets/130823585/d3f8de18-49ca-434f-bc02-e7360b7ae377">

thank you hope this what helpful
  


