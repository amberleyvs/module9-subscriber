## Questions

**a. How much data will the publisher program send to the message broker in one run?**

The publisher program will send 5 data messages to the message broker in one run.

This happens because the program calls `publish_event` five times. Each `publish_event` call sends one `UserCreatedEventMessage` to RabbitMQ through the `user_created` queue.

**b. The URL `amqp://guest:guest@localhost:5672` is the same as in the subscriber program. What does it mean?**

It means that both the publisher and subscriber connect to the same RabbitMQ message broker.

In the URL:

- `amqp://` means the program uses the AMQP protocol.
- The first `guest` is the username.
- The second `guest` is the password.
- `localhost` means RabbitMQ is running on the same computer.
- `5672` is the default port used by RabbitMQ for AMQP communication.

Because the publisher and subscriber use the same URL, the publisher can send messages to RabbitMQ, and the subscriber can receive messages from the same RabbitMQ broker.