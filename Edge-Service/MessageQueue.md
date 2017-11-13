# Message Queue
TODO: 
- Architecture Diagram

## Overview
### Pika Library
### AMQP Library -- Front end docs
### RabbitMQ on Cloud

## Queue Capabilities
### Connection
### Create Queue 
### Delete Queue
### Send Message
#### Request
Request Body
```javascript
{
  "properties":{},
  "routing_key":"goalScored",
  "payload":{"left": Boolean, "right": Boolean},
  "payload_encoding":"json"
}
```
### Receive Message -- front end docs
