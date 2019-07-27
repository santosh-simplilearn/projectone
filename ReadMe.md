
# To dockerize apache and deploy a sample index.html page follow below steps


## 1) Run below command to git pull "santosh-project" repo into the jenkins workspace
    ```
    For now ignore this step
    ```
## 2) Run below command to create  a docker build
    ```
    docker build -t centos7/samplewebpage:latest -f=Dockerfile .
    ```
## 3) Run below command to run the docker container
    ```
    docker run -d -p 3000:80 centos7/samplewebpage:latest
    ```
## 4) Run below command to see if the conainer is running or not
    ```
    docker ps
    ```

## 5) Open below URL in a browser and you should see Hello World Sample HTML Page
    ```
    http://localhost:3000
    ```