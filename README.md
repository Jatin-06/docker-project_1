# docker-project_1

HISTORY
docker pull nginx:stable-alpine3.17-slim
docker run -d -p 8080:80 nginx:stable-alpine3.17-slim
docker --help
docker exec --help
docker ps
docker exec 9008825ac8f3 cat /etc/os-release
docker exec 9008825ac8f3 cat /etc/os-release | grep -i pretty
docker exec --help
docker exec -it 9008825ac8f3 sh
docker ps
mkdir test
cd test
git clone https://github.com/Jatin-06/docker-project_1.git
cd web
ls
docker --help
docker cp --help
ls
docker ps
docker cp colors.css 9008825ac8f3:/usr/share/nginx/html
docker cp colors.js 9008825ac8f3:/usr/share/nginx/html
docker cp index.html 9008825ac8f3:/usr/share/nginx/html
Open browser hit ip:portnumber
