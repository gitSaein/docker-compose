RabbitMQ


1. RabbitMQ Clustering
$ docker exec -ti rabbitmq_node2 bash -c "rabbitmqctl stop_app"
$ docker exec -ti rabbitmq-node2 bash -c "rabbitmqctl join_cluster rabbit@rabbitmq_node1"
$ docker exec -ti rabbitmq-node2 bash -c "rabbitmqctl start_app"
$ docker exec -ti rabbitmq-node2 bash -c "rabbitmqctl cluster_status"