#### 仓库
~~~
docker login x.x -u *** -p ***
docker tag mattermost/mattermost-prod-app:3.7.3 x.x/mattermost/mattermost-app:3.7.3
docker push x.x/mattermost/mattermost-app:3.7.3
~~~

#### 容器
docker run -d -p 8083:8083 -p 8086:8086 --expose 8090 --expose 8099 --name influxdb tutum/influxdb:0.8.8
docker attach containerId
Ctrl+d
docker rm containerId
docker rm -f `docker ps -aq`

#### influxdb
influx
use influxdb
SHOW MEASUREMENTS



