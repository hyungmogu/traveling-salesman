# Traveling Salesman
Author's demonstration of algorithm skills. Returns near-shortest circular path of 30 locations. This app mimicks the path finding service used by Amazon delivery vehicles and FedEx. 

Traveling salesman problem related algorithm is computationally intensive. The least desired scenario is sending a request and wait for 5+ minutes. C++ is being used to boost the time taken to process the algorithm. The choice is deliberate to increase the number of requests handled per server.

Apache Kafka is used to handle a large number of requests. Once a user (consumer) is subscribed to Apache Kafka (by requesting for shortest path of x points), producer (This application) solves the traveling salesman problem of x points, and it sends response back to consumer. Apache Kafka is a perfect choice to handle requests for this application where a large numbet of some time-consuming requests are required.

# Requirements and Resource Estimation

# Diagrams

# References

