# Camel-infinispan-idempotent
Simple project demonstrating how to use:
  Apache Camel + Infinispan + Idempotent Consumer(EIP)

# Technologies
- Java8
- Apache Camel
- Infinispan


# Idempotent Consumer
The Idempotent Consumer from the EIP patterns is used to filter out duplicate messages.

This pattern is implemented using the IdempotentConsumer class. This uses an Expression to calculate a unique message ID string for a given message exchange; this ID can then be looked up in the IdempotentRepository to see if it has been seen before; if it has the message is consumed; if its not then the message is processed and the ID is added to the repository.

Link: http://camel.apache.org/idempotent-consumer.html


# Infinispan
Infinispan is a distributed in-memory key/value data store with optional schema, available under the Apache License 2.0.

Link: http://infinispan.org/
