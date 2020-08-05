# Stock App
Phase3 Stock Application

## Microservices Names-
### 1. feign-service
#### Endpoints- 
- feign/{compId}   
  Method - GET  
  Returns company with company ID
- feign/matching/{compName}  
  Method - GET  
  Returns list of companies with company Name pattern
- feign/ipos/{compName}  
  Method - GET  
  Returns ipo with given company Name
- feign/sector/{compName}  
  Method - GET  
  Returns sector with given company Name
- feign/se/{se}
  Method - GET  
  Returns list of companies with given Stock Exchange
- feign/se-service/{seId}
  Method - GET  
  Returns the Stock Exchange object with the given seId
- feign/se-service
  Method - GET  
  Returns list of all Stock Exchange object
- feign/add  
  Method - POST  
  Add the company details to the database
- feign/se-service/  
  Method - POST  
  Add the stock exchange details to the database
#### SWAGGER Screenshots-
![](images/feign-swagger-ss-1.png)

![](images/feign-swagger-ss-2.png)

### 2. Eureka Discovery Service-
#### Screenshots- 
![](images/eureka-discovery-service-ss-1.png)

![](images/eureka-discovery-service-ss-2.png)

### 3. company-details
#### Endpoints-
- companies/{compId}  
  Method - GET  
  Returns company with company ID
- companies/matching/{compName}  
  Method - GET  
  Returns list of companies with company Name pattern
- companies/sector/{sector}  
  Method - GET  
  Returns list of companies in given sector
- companies/se/{se}
  Method - GET  
  Returns list of companies with given Stock Exchange
- companies/add  
  Method - POST  
  Add the company details to the database
#### SWAGGER Screenshots- 
![](images/company-details-swagger-ss-1.png)

![](images/company-details-swagger-ss-2.png)

### 4. ipo-service
#### Endpoints-
- ipos/{compId}  
  Method - GET  
  Returns list of ipos using company ID
#### SWAGGER Screenshots-
![](images/ipo-swagger-ss-1.png)

### 5. se-service
#### Endpoints-
- /se/{seId}  
  Method - GET  
  Returns the Stock Exchange object with the given seId
- /se/  
  Method - POST  
  Add the stock exchange details to the database
- /se  
  Method - GET  
  Returns list of all Stock Exchange object
#### SWAGGER Screenshots-  
![](images/se-service-swagger-ss-1.png)

### 6. ADMIN Server
#### Screenshots- 
![](images/admin-service-ss-1.png)

![](images/admin-service-ss-2.png)

### 7. config-server

### 8. ZIPKIN-
- JAR Link- https://drive.google.com/file/d/1cIAdvxKvXb9Uqv6b4Edce7aCfD1042_k/view?usp=sharing
#### Screenshots- 
![](images/zipkin-ss-1.png)

![](images/zipkin-ss-2.png)

### SWAGGER In Action-
![](images/swagger-in-action-ss-1.png)

![](images/swagger-in-action-ss-2.png)

## DEPLOYMENT (AWS)-
- Link- http://stockappcompanydetails-env.eba-ezmrrzpn.ap-south-1.elasticbeanstalk.com/companies/100
- Swagger Link - http://stockappcompanydetails-env.eba-ezmrrzpn.ap-south-1.elasticbeanstalk.com/swagger-ui.html

## USER INTERFACE (Angular)-  
#### Stock Exchange List Page
![](images/ui-ss-1.png)

#### Add Stock Exchange Page
![](images/ui-ss-2.png)

![](images/ui-ss-3.png)

#### Update Stock Exchange List Page  
![](images/ui-ss-4.png)


## JMeter Testing Screenshots  
<p float="left">
  <img src="/images/testing-ss-1.png" width="45%" />
  <img src="/images/testing-ss-2.png" width="45%" /> 
</p>

<p float="left">
  <img src="/images/testing-ss-3.png" width="45%" />
  <img src="/images/testing-ss-4.png" width="45%" /> 
</p>

<p float="left">
  <img src="/images/testing-ss-5.png" width="45%" />
</p>

## Docker  
Docker implementation of company-service.
- DockerHub link to run the service- docker pull anshul16/company-details  
- Port used-5000
- Use http://localhost:5000/swagger-ui.html to run on local machine.
#### Screenshot
![](images/docker-image-ss-1.png)
