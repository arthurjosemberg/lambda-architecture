# Listar todos os Topicos
$CONFLUENT_HOME/bin/kafka-topics --list  \
--zookeeper node-01.localdomain:2182

# Deletar um topico
$CONFLUENT_HOME/bin/kafka-topics --delete \
--zookeeper node-01.localdomain:2182 \
--topic [Topic Name]

# Criar um topico
$CONFLUENT_HOME/bin/kafka-topics --create \
--zookeeper node-01.localdomain:2182 \
--replication-factor 1 \
--partitions 1 \
--topic [Topic Name]