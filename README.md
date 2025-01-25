# Real-Time-E-Commerce-Analytics-Pipeline

## Project Overview
Real-time data processing pipeline for e-commerce events using Scala, Apache Kafka, and Spark Streaming.

## Technologies Used
- Scala 2.13.x
- Apache Kafka
- Apache Spark Streaming
- PostgreSQL

## Features
- Real-time event ingestion
- Stream processing
- Metrics computation
- Database storage

## Prerequisites
- Scala 2.13.x
- Kafka 2.8+
- Spark 3.2+
- PostgreSQL 12+

## Installation

### 1. Clone Repository
```bash
git clone https://github.com/yourusername/ecommerce-analytics.git
cd ecommerce-analytics
```

### 2. Setup Dependencies
```bash
sbt clean compile
```

### 3. Configure Kafka
- Create Kafka topic: `ecommerce-events`
- Update `bootstrap.servers` in code

### 4. Configure PostgreSQL
- Create database: `ecommerce_metrics`
- Update connection parameters

## Running the Project
```bash
# Start Kafka
bin/kafka-server-start.sh config/server.properties

# Start Spark Streaming Job
sbt run
```

## Project Structure
```
src/
├── main/
│   ├── scala/
│   │   ├── EcommerceEvent.scala
│   │   ├── KafkaEventProducer.scala
│   │   └── EcommerceStreamingAnalytics.scala
└── test/
    └── scala/
        └── EcommerceAnalyticsSpec.scala
```

## Configuration
- `application.conf`: Project configurations
- `logback.xml`: Logging configurations

## Monitoring
- Kafka: Offset tracking
- Spark: Web UI (http://localhost:4040)

## Scaling Strategies
- Horizontal Kafka scaling
- Spark cluster mode
- Distributed processing

## Contributing
1. Fork repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Create pull request

- Email: apaliwal@ee.iitr.ac.in
