# stock-app
Phase3 Stock App

Microservices Names-
1. feign-service
Endpoints- 
- feign/{compId} GET returns company with company ID
- feign/matching/{compName} GET reuters list of companies with company Name pattern
- feign/ipos/{compName} GET returns ipo with given company Name
- feign/sector/{compName} GET returns sector with given company Name
- feign/se/{se} GET returns list of companies with given Stock Exchange
- feign/se-service/{seId} GET returns the Stock Exchange object with the given seId
- feign/se-service GET returns list of all Stock Exchange object
- feign/add POST add the company details to the database
- feign/se-service/ POST add the stock exchange details to the database
SWAGGER Screenshots-

2. eureka-discovery-service 
3. company-details
Endpoints-
- companies/{compId} GET returns company with company ID
- companies/matching/{compName} GET reuters list of companies with company Name pattern
- companies/sector/{sector} GET returns list of companies in given sector
- companies/se/{se} GET returns list of companies with given Stock Exchange
- companies/add POST add the company details to the database
  SWAGGER Screenshots- 

4. ipo-service
Endpoints-
- ipos/{compId} GET returns list of ipos using company ID
SWAGGER Screenshots-

5. se-service
Endpoints-
- /se/{seId} GET  GET returns the Stock Exchange object with the given seId
- /se/  POST add the stock exchange details to the database
- /se GET returns list of all Stock Exchange object
SWAGGER Screenshots-  

6. admin-server
7. config-server

USER INTERFACE (Angular)-

DEPLOYMENT (AWS)-
Link- http://stockappcompanydetails-env.eba-ezmrrzpn.ap-south-1.elasticbeanstalk.com/companies/100
Swagger Link - http://stockappcompanydetails-env.eba-ezmrrzpn.ap-south-1.elasticbeanstalk.com/swagger-ui.html
SWAGGER In Action-

ADMIN Service-

Eureka Discovery Service-

ZIPKIN-

USER INTERFACE (Angular)-  
Stock Exchange List Page

Add Stock Exchange Page

Update Stock Exchange List Page  


