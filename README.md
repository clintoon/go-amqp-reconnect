# rabbitmq/amqp091-go Conneciton/Channel auto reconnect wrap
rabbitmq/amqp091-go Connection/Channel does not reconnect if rabbitmq server restart/down.

To simply developers, here is auto reconnect wrap with detail comments.

## How to change existing code
1. add import `import "github.com/clintoon/go-amqp-reconnect/rabbitmq"`
2. Replace `amqp.Connection`/`amqp.Channel` with `rabbitmq.Connection`/`rabbitmq.Channel`!

## Example
### Close by developer
> go run example/close/demo.go

### Auto reconnect
> go run example/reconnect/demo.go

