# kafka命令

显示当前的topic

```shell
kafka-topics --list --zookeeper 172.16.8.38:2181,172.16.8.39:2181,172.16.8.40:2181/kafka 

```



创建topic

```shell
kafka-topics --create --zookeeper 172.16.8.38:2181,172.16.8.39:2181,172.16.8.40:2181/kafka --replication-factor 1 --partitions 1 --topic test
```

kafka生产者客户端命令

```
kafka-console-producer --broker-list 172.16.8.40:9092 --topic test
```

kafka消费者客户端命令

```
kafka-console-consumer --bootstrap-server 172.16.8.40:9092 --from-beginning --topic test

kafka-console-consumer --bootstrap-server 172.16.8.40:9092 --from-beginning --topic nginx170


```

