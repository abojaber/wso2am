# wso2 API Management
run wso2am on docker


## Running WSO2AM
- Before start: download wso2am [API Management](https://wso2.com/api-management/) into `./wso2am` 
	- If you run macOS or windows you may use docker-machine.

###steps:
- clone the project: `https://github.com/abojaber/wso2am.git`
- copy the downloaded file to wso2am/wso2am/
- start your docker-machine & set the enviroment 
- go to wso2am `cd wso2am` 
- build the image: `docker build wso2am . `
- start the container: `docker run -p 9443:9443 -p 9763:9763 -p 8243:8243 -p 8280:8280 -p 10397:10397 -p 7711:7711 wso2am `
- now you can access the wso2am using machine-ip

## issue:
- if you need to now your docker-machine ip ` docker-machine env <machine-name>`
### Reference
- [Run WSO2 Api Manager with Docker](https://malalanayake.wordpress.com/2018/01/11/run-wso2-api-manager-with-docker/)
- [Docker Get Start](https://docs.docker.com/get-started/)
- [Docker Machine](https://docs.docker.com/machine/)