# wso2 API Management
run wso2am on docker


## Running WSO2AM
- Before start: download wso2am [API Management](https://wso2.com/api-management/) into `./wso2am` 
	- If you run macOS or windows you may use docker-machine.

###steps:
- clone the project: `https://github.com/abojaber/wso2am.git`
- download wso2am-2.1.0.zip from https://github.com/wso2/product-apim/releases 
- copy the downloaded file to wso2am/wso2am/
- start your docker-machine & set the enviroment 
- go to wso2am `cd wso2am` 
- build the image: `docker build . -t wso2am`
- start the container: `docker run -p 9443:9443 -p 9763:9763 -p 8243:8243 -p 8280:8280 -p 10397:10397 -p 7711:7711 wso2am `
- wait for 2~ min  :) 
- now you can access the wso2am using machine-ip

publisher link: (https://<hostname>:9443/publisher)

store link: (https://<hostname>:9443/store)
## issue:
- if you need to now your docker-machine ip ` docker-machine env <machine-name>`
- to check the log you may run `docker logs <containerID> -f`
### Reference
- [Run WSO2 Api Manager with Docker](https://malalanayake.wordpress.com/2018/01/11/run-wso2-api-manager-with-docker/)
- [Docker Get Start](https://docs.docker.com/get-started/)
- [Docker Machine](https://docs.docker.com/machine/)
- [wso2 API Manager Tutorials](https://docs.wso2.com/display/AM210/Tutorials)
