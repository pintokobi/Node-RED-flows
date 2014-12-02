Name:
=====

Pub/Sub using RabbitMQ.

Principal Nodes:
================

* inject
* RabbitMQ out
* RabbitMQ in
* function
* delay
* debug

Explanation:
============

This flow Using RabbitMQ out Client to publish data and RabbitMQ in client to subscribe to the queue
for received the data and display in debug.

Prerequisites/Preconditions/Assumptions:
========================================
NA

General Flow Description :
=========================

Classic pub/sub interaction. 
Using RabbitMQ out Client to send data to RabbitMQ in client and display in debug the received data.

Detailed Implementation:
========================

* inject       - setting the message we want to send.
* RabbitMQ out - client to publish message for specified queue.
* RabbitMQ in  - client to subscribe to specified queue  for receiving message.
* function     - use acknowledge to get the next message in the queue.
* delay        - use to keep message in queue so we can see it works properly.
* debug        - display the msg.payload output.  

Additional or Useful Info:
==========================

this flow using this links:
RabbitMQ Management: http://10.112.10.72:15672/
go to Queues tab and see the traffic while pressing on the inject nodes.



+[![Build Status]http://upload.wikimedia.org/wikipedia/commons/d/da/Kobi_perez.jpg]+
