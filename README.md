# Redis – Getting Started

## You Need:

* Linux or Mac machine
* Docker installed & running
* Terminal Application
* Or simply use the [Google Cloud Shell](https://console.cloud.google.com/home/dashboard?cloudshell=true) (free!)

## 1 – Run Redis with Interactive Shell

`git clone https://github.com/u1i/redis-getting-started`

`cd redis-getting-started`

`./run-redis.sh`

## 2 – Get & Set Values

### Set a Key
`set student kelly`

> OK

### Get the Value of that Key
`get student`

> "kelly"

## 3 – Working with Lists

### Add a value to the 'queue'
`lpush message_queue hello`

### Add one more
`lpush message_queue "hello again"`

### Retrieve the 'oldest' value in the 'queue'

`rpop message_queue`

> "hello"

Now when we do that again....

`rpop message_queue`

> "hello again"

And one more time:

`rpop message_queue`

> (nil)

## 4 – Working with Increments

`incr queue_number`
> (integer) 1

`incr queue_number`
> (integer) 2






