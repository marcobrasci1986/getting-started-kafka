## Produce

    kafka-console-producer --bootstrap-server 127.0.0.1:9092 --topic first_topic

## Consume

    kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic first_topic --from-beginning

## Create a topic

    kafka-topics --create --bootstrap-server 127.0.0.1:9092 --replication-factor 1 --partitions 3 --topic myorders

## Reassign partitions

    kafka-reassign-partitions --bootstrap-server 127.0.0.1:9092 --reassignment-json-file increase_replication.json --execute
