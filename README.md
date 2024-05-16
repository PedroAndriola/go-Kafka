go-Kafka

Este repositório contém um exemplo de aplicação Go para consumir mensagens de um cluster Kafka usando a biblioteca Sarama.

Instruções de Uso
Pré-requisitos
Certifique-se de ter o Docker e o Docker Compose instalados em sua máquina.
Configuração do Ambiente
Clone este repositório em sua máquina local:

git clone https://github.com/seu-usuario/go-Kafka.git
Navegue até o diretório clonado:
cd go-Kafka
Execução
Inicie o ambiente usando o Docker Compose:

docker-compose up -d
Aguarde até que todos os serviços estejam prontos. Você pode verificar o status dos serviços executando:


docker-compose ps
Após todos os serviços estarem prontos, execute a aplicação Go Kafka Consumer:

go run main.go
Isso iniciará o consumidor Kafka, que estará pronto para receber mensagens do tópico "topic-test" no cluster Kafka.

Você verá as mensagens sendo impressas no console conforme são consumidas.

Acesso à Interface Conduktor
Após iniciar o ambiente, você pode acessar a interface do Conduktor em http://localhost:8080. Isso fornecerá uma visualização do cluster Kafka e outras métricas relacionadas.

Nota Importante
Este ambiente é destinado apenas para fins de demonstração e aprendizado. Não é adequado para uso em produção. Certifique-se de revisar as configurações e adaptá-las conforme necessário para o seu ambiente de produção.

Para ambientes de produção, consulte a documentação oficial do Conduktor para opções de implantação adequadas: Documentação do Conduktor - Opções de Implantação.
