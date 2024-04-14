This is a fork of the Confluent Kafka REST Proxy project. The original project can be found at https://github.com/confluentinc/kafka-rest

This produces custom headers based also on all the http headers:

```shell
cucurl -X POST -H "Content-Type: application/json" -H "X-Test: hello" \      
-d '{"value":{"type":"JSON","data":{"name":"testUser"}}}' \       
http://localhost:8082/v3/clusters/f8XrShmLQfCQmPRj2fHYKw/topics/jsontest/records
```