Node.js code for RabbitMQ tutorials
Here you can find JavaScript (Node) code examples from RabbitMQ tutorials.

To successfully use the examples you will need a running RabbitMQ server.

Requirements
Node.js
You need Node.js and amqp.node to run these tutorials.

Client Library
To install amqp.node using npm:

npm install amqplib -g

code -

Tutorial two: Work Queues:

node src/new_task.js "A very hard task which takes two seconds.."
node src/worker.js

Tutorial three: Publish/Subscribe

node src/receive_logs.js
node src/emit_log.js "info: This is the log message"

Tutorial four: Routing:

node src/receive_logs_direct.js info
node src/emit_log_direct.js info "The message"

Tutorial five: Topics:

node src/receive_logs_topic.js "*.rabbit"
node src/emit_log_topic.js red.rabbit Hello

Tutorial six: RPC:

node src/rpc_server.js
node src/rpc_client.js 30