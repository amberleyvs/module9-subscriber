# Tutorial A: Event-Driven Architecture

**1. What is AMQP?**

AMQP stands for Advanced Message Queuing Protocol. It is a messaging protocol used by applications to communicate through a message broker. In this tutorial, AMQP is used so the publisher and subscriber can communicate through RabbitMQ without directly calling each other.

**2. What does it mean? guest:guest@localhost:5672 , what is the first guest, and what is the second guest, and what is localhost:5672 is for?**

The first guest is the username used to connect to RabbitMQ.

The second guest is the password used to connect to RabbitMQ.

localhost:5672 means the RabbitMQ server is running on the local computer, and the application connects to it through port 5672. Port 5672 is the default port used by RabbitMQ for AMQP communication.