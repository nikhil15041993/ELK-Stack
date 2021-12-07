# ELK-Stack


The ELK Stack is a collection of three open-source products — Elasticsearch, Logstash, and Kibana. ELK stack provides centralized logging in order to identify problems with servers or applications.

![Test Image 5](https://miro.medium.com/max/1024/0*oU6HEQfPfyF689QF.png)



## How To Create A Pipeline In Logstash
 ## What Is A Logstash Pipeline:
The Logstash event processing pipeline has three stages: inputs ==> filters ==> outputs. Inputs generate events, filters modify them and outputs ship them elsewhere. Inputs and outputs support codecs that enable you to encode or decode the data as it enters or exits the pipeline without having to use a separate filter.


## Logstash Pipeline Stages:
## Inputs:
Inputs are used to get data into Logstash. Logstash supports different input as your data source, it can be a plain file, syslogs, beats, cloudwatch, kinesis, s3, etc.

## Filters:
Filters are intermediary processing devices in the Logstash pipeline. You can combine filters with conditionals to perform an action on an event if it meets certain criteria. Logstash supports different types of filters for data processing like gork, mutate, aggregate, csv, json, etc.

## Outputs:
Outputs are the final phase of the Logstash pipeline. An event can pass through multiple outputs, but once all output processing is complete, the event has finished its execution. Logstash supports different types of outputs to store or send the final processed data like elasticsearch, cloudwatch, csv, file, mongodb, s3, sns, etc.

```
# example pipeline config file format
input {
  ...
  codec {
    ...
  }
}
filter {
  ...
}
output {
  ...
  codec {
    ...
  }
}
```
