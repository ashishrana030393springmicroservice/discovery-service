###Eureka client
* eureka client sends heart beat  in every 30 seconds to eureka server
* lease-renewal-interval-in-seconds: it sets heart beat interval
* it will try to fetch registry from eureka server and cache it, fetch-registry is true by default
* it will register itself with eureka server, register-with-eureka is true by default
* /eureka/apps is a endpoint in eureka server, through which eureka client fetches registry
###Eureka server
* eureka server removes the instance if it didn't receive any heart beat for 90 seconds
* lease-expiration-duration-in-seconds: it sets service expiry period
