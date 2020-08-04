# Stock App
Phase3 Stock Application

## Microservices Names-
### 1. feign-service
#### Endpoints- 
- feign/{compId} GET returns company with company ID
- feign/matching/{compName} GET reuters list of companies with company Name pattern
- feign/ipos/{compName} GET returns ipo with given company Name
- feign/sector/{compName} GET returns sector with given company Name
- feign/se/{se} GET returns list of companies with given Stock Exchange
- feign/se-service/{seId} GET returns the Stock Exchange object with the given seId
- feign/se-service GET returns list of all Stock Exchange object
- feign/add POST add the company details to the database
- feign/se-service/ POST add the stock exchange details to the database
#### SWAGGER Screenshots-
![](images/feign-swagger-ss-1.png)

![](images/feign-swagger-ss-1.png)

### 2. Eureka Discovery Service-
#### Screenshots- 
![](images/eureka-discovery-service-ss-1.png)

![](images/eureka-discovery-service-ss-2.png)

### 3. company-details
#### Endpoints-
- companies/{compId} GET returns company with company ID
- companies/matching/{compName} GET reuters list of companies with company Name pattern
- companies/sector/{sector} GET returns list of companies in given sector
- companies/se/{se} GET returns list of companies with given Stock Exchange
- companies/add POST add the company details to the database
#### SWAGGER Screenshots- 
![](images/company-details-swagger-ss-1.png)

![](images/company-details-swagger-ss-2.png)

### 4. ipo-service
#### Endpoints-
- ipos/{compId} GET returns list of ipos using company ID
#### SWAGGER Screenshots-
![](images/ipo-swagger-ss-1.png)

### 5. se-service
#### Endpoints-
- /se/{seId} GET  GET returns the Stock Exchange object with the given seId
- /se/  POST add the stock exchange details to the database
- /se GET returns list of all Stock Exchange object
#### SWAGGER Screenshots-  
![](images/se-service-swagger-ss-1.png)

### 6. ADMIN Server
#### Screenshots- 
![](images/admin-service-ss-1.png)

![](images/admin-service-ss-2.png)

### 7. config-server

### 8. ZIPKIN-
#### Screenshots- 
![](images/zipkin-ss-1.png)

![](images/zipkin-ss-2.png)

## DEPLOYMENT (AWS)-
- Link- http://stockappcompanydetails-env.eba-ezmrrzpn.ap-south-1.elasticbeanstalk.com/companies/100
- Swagger Link - http://stockappcompanydetails-env.eba-ezmrrzpn.ap-south-1.elasticbeanstalk.com/swagger-ui.html

### SWAGGER In Action-
![](images/swagger-in-action-ss-1.png)

![](images/swagger-in-action-ss-2.png)

## USER INTERFACE (Angular)-  
#### Stock Exchange List Page
![](images/ui-ss-1.png)

#### Add Stock Exchange Page
![](images/ui-ss-2.png)

![](images/ui-ss-3.png)

#### Update Stock Exchange List Page  
![](images/ui-ss-4.png)

