# docker-project_1
below is manual step, after that we will see making Dockerfile and expose container to outside world, steps are below manual!!

HISTORY <br>
docker pull nginx:stable-alpine3.17-slim <br>
docker run -d -p 8080:80 nginx:stable-alpine3.17-slim <br>
docker --help <br>
docker exec --help <br>
docker ps <br>
docker exec 9008825ac8f3 cat /etc/os-release <br>
docker exec 9008825ac8f3 cat /etc/os-release | grep -i pretty <br>
docker exec --help <br>
docker exec -it 9008825ac8f3 sh <br>
docker ps <br> 
mkdir test <br> 
cd test <br> 
git clone https://github.com/Jatin-06/docker-project_1.git <br>
cd web <br> 
ls <br> 
docker --help <br> 
docker cp --help <br> 
ls <br> 
docker ps <br> 
docker cp colors.css 9008825ac8f3:/usr/share/nginx/html <br> 
docker cp colors.js 9008825ac8f3:/usr/share/nginx/html <br> 
docker cp index.html 9008825ac8f3:/usr/share/nginx/html <br> 
Open browser hit ip:portnumber <br> 

Now we will Deploy app by Creating Dockerfile <br>
FROM ubuntu  <br>
RUN apt update && apt install nginx -y <br>
COPY . /var/www/html  <br>
CMD nginx -g 'daemon off;'    //this command will stop daemon so that it wont run in background. We want nginx to run in foreground <br>

docker build . -t swizzy      //this command will make image

