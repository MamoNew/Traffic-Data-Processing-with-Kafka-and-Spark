## Traffic Data Processing with Kafka and Spark 🚗📊

This project demonstrates a pipeline for real-time traffic data processing using Kafka and Spark. The system includes components for data generation, Kafka message production, Spark Structured Streaming, and Spark ML integration.

### 1. *Traffic Data Generation 🚦*

The first part of the project involves generating simulated traffic data from a CSV file. The Python script TrafficDataGenerator.py utilizes Pandas to read a CSV file and push each row as a JSON message to a Kafka topic.

![Traffic Data Generation](<insert_image_url_here>)

### 2. *Spark Structured Streaming 🌟*

The Spark Structured Streaming script (StructuredStreaming.py) subscribes to the Kafka topic, processes incoming JSON messages, and applies streaming analytics. The processed data is then filtered based on a condition (e.g., Total > 50) and displayed on the console.

![Spark Structured Streaming](<insert_image_url_here>)

### 3. *Spark ML Integration 🤖*

The next step involves machine learning integration using Spark ML. The script SparkMLIntegration.py reads streaming data and combines it with static data for training a Linear Regression model. The model is then used to make predictions on the streaming data, and the results are displayed.

![Spark ML Integration](<insert_image_url_here>)

### 4. *Kafka Message Producer with Limit ⏰*

To control the duration of data production, the script KafkaMessageProducerWithLimit.py sends data to Kafka for a specified duration. This can be useful for testing and limiting the amount of data pushed to Kafka.

![Kafka Message Producer with Limit](<insert_image_url_here>)

### 5. *Upload Dataset to Kafka Procedure 🔄*

The UploadDatasetToKafkaProcedure.py script demonstrates a Kafka consumer that subscribes to the topic and continuously polls for messages. Received messages are printed to the console, and this process can run indefinitely.

![Upload Dataset to Kafka Procedure](<insert_image_url_here>)

### 6. *Additional Scripts 🧰*

- KafkaProducer.py: Basic Kafka producer setup.
- SparkGraphX.py: A script using GraphFrames for graph processing.
- SparkSQL.py: A script demonstrating Spark SQL processing on streaming data.

Feel free to explore each script based on your project's requirements. Happy coding! 🚀
