# Real-Time-Streaming-of-Transactional-data-at-Scale
Real time streaming of fake transactional data at scale by Integrating Apache Flink, Kafka, Postgres, Elasticsearch, Kibana, and Docker

![image](https://github.com/Ndaruga/Real-Time-Streaming-of-Transactional-data-at-Scale/assets/68260816/23551617-fa28-4fa0-b497-c1db715e6eb0)


### The Components
* **Apache Kafka:** It can handle huge amounts of data constantly flowing in (like a stream) and out (publish and subscribe). It can also temporarily store this data and even process it while it's flowing through.
* **Apache Flink:** This is like a powerful factory for real-time data processing. It can continuously analyze endless streams of data (unbounded) or even fixed datasets (bounded) with high speed and very little delay.
* **PostgreSQL (Postgres):** This is a superstar among databases, known for its reliability, richness in features, and overall speed.
* **Elasticsearch:**  It's spread across multiple machines (distributed) and can be used for many different tasks, not just searching. Plus, it offers a user-friendly interface for interacting with it.
* **Kibana:** A tool specifically designed to visualize data from Elasticsearch. It takes all the information Elasticsearch has stored and turns it into charts, graphs, and other visual formats for you to explore easily.

## Setting up the System Architecture 
1. Clone this repository from GitHub
2. To begin, ensure you have Docker installed on your system. Ensure that the file `docker-compose.yml` exists. Docker Compose will allow us to define and run multi-container Docker applications. 

    ```
    docker compose up -d
    ```
3. 
