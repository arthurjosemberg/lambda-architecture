# Comando usado para criar o debezium source connector
# O arquivo deve estar no diretório $CONFLUENT_HOME/etc/kafka/
./bin/confluent load debezium-connector-postgresql -d ./etc/kafka/debezium-connector-postgres.json

# Comando usado para validar a criação do debezium source connector
./bin/confluent status debezium-connector-postgresql

# Comando usado para excluir o debezium source connector
./bin/confluent unload debezium-connector-postgresql

###########################################################################

# Comando usado para criar o hdfs sink connector
# O arquivo deve estar no diretório $CONFLUENT_HOME/etc/kafka-connect-hdfs/
./bin/confluent load hdfs-sink-connector -d ./etc/kafka-connect-hdfs/hdfs-sink-connector.json

# Comando usado para validar a criação do hdfs sink connector
./bin/confluent status hdfs-sink-connector

# Comando usado para excluir o hdfs sink connector
./bin/confluent unload hdfs-sink-connector



