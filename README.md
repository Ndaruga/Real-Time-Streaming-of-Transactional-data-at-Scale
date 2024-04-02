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
3. Next, You need to set up **Apache Flink** preferably version 1.18.* for this project
   *    Apache Flink will run on all UNIX systems including MacOS. If you are on Windows, It is advisable to install Windows Subsystem for Linux (WSL) from Microsoft.
   *    You need to have `Java 11` installed in your system. You can check the java version by running the command
           ```
           java --version
           ```
   *    Download the [latest binary release of Flink](https://flink.apache.org/downloads.html), then extract the archive:
           ```
           tar -xvf flink-<flink version>.tgz
           ```
       
   *    To test if your Flink cluster is running locally, navigate to the extracted flink folder run the command
         ```
         ./bin/start-cluster.sh
         ```
         Once the cluster has started, you can view the flink dashboard [http://localhost:8081](http://localhost:8081) and you should see a dashboard such as this

        <img width="1200" alt="Screenshot 2024-04-02 at 10 47 43 PM" src="https://github.com/Ndaruga/Real-Time-Streaming-of-Transactional-data-at-Scale/assets/68260816/0d43ecde-d5a7-416a-9a18-1e023acf55fb">

        To stop the cluster run
        ```
        ./bin/stop-cluster.sh
        ```

