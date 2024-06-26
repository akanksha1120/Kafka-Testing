Kafka Producer and Consumer Example

Prerequisites
Before running the producer and consumer, ensure you have the following installed:

Node.js
npm (Node Package Manager)
Kafka running locally or accessible via specified brokers
Setup

1. Clone the repository:
   git clone https://github.com/akanksha1120/Kafka-Testing.git
   cd Kafka-Testing

2. Install dependencies:
   npm install

3. Configuration: Update the Kafka broker configuration in producer.js and consumer.js files if necessary:

const kafka = new Kafka({
clientId: 'your-client-id',
brokers: ['localhost:9092'] // Update with your Kafka broker(s) address
});

Running the Producer
The producer sends random animal names to the Kafka topic "animals" at an interval of 1 second.
To run the producer, execute:

-> [node producer.js]

Running the Consumer
The consumer listens to the "animals" topic and prints received messages to the console.
To run the consumer, execute:

-> [node consumer.js]

Notes
Ensure Kafka is running and accessible at the specified broker address (localhost:9092 by default).
Modify the topic name, broker addresses, and other configurations as per your Kafka setup.
