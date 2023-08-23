# Traveling Salesman
Author's demonstration of algorithm skills. Returns near-shortest circular path of 30 locations. This app mimicks the path finding service used by Amazon delivery vehicles and FedEx. 

Traveling salesman problem related algorithm is computationally intensive. The least desired scenario is sending a request and wait for 5+ minutes. C++ is being used to boost the time taken to process the algorithm. The choice is deliberate to increase the number of requests handled per server.

Apache Kafka is used to handle a large number of requests. Once a user (consumer) is subscribed to Apache Kafka (by requesting for shortest path of x points), producer (This application) solves the traveling salesman problem of x points, and it sends response back to consumer. All the details of Kafka events are stored in a hard drive. In sum, request bottleneck and the likelihood of server crashing (due to little RAM remaining) is reduced. Apache Kafka is a perfect choice to handle requests for this application where there are a large number of some time-consuming requests.

# Requirements and Resource Estimation

# Diagrams

# References

