# Anotações de Estudo com IA (Spring AI)

Sistema web simples feito com **Spring Boot + Spring AI**.
É possivel inserir anotações de estudo e usa a GenAI para **resumir**, **gerar perguntas de estudo** e **perguntar sobre o conteúdo** da nota.

# Funcionalidades 
- Criar, editar e excluir anotações.
- Gerar resumos utilizando inteligência artificial.
- Gerar perguntas para revisão de conteúdo.
- Fazer perguntas sobre o conteúdo de uma anotação.
- Armazenar as anotações em banco de dados.
- Utilizar inteligência artificial local por meio do Ollama.

# Requisitos
- Java JDK 17 ou superior
- Maven
- Ollama

# Banco de Dados
O projeto utiliza o H2 Database, configurado para armazenar os dados localmente em arquivo.
As anotações são armazenadas no diretório data, permitindo que os dados permaneçam salvos após o encerramento da aplicação.

# Inteligência Artificial 
A aplicação utiliza o Ollama para executar modelos de inteligência artificial localmente.
A comunicação ocorre por meio da API local do Ollama, no endereço: http://localhost:11434
O modelo utilizado é o Qwen 2.5 3B.
A integração permite gerar resumos, perguntas de estudo e respostas baseadas no conteúdo das anotações, sem necessidade de uma chave de API externa.

# E caso queira executar: 

-Clone o repositório e entre na pasta do projeto -> cd notas-ia
-Instale o Ollama no site oficial deles -> [https://ollama.com/download](url)
-Baixe o modelo de IA -> ollama run qwen2.5:3b
-Execute a aplicação -> mvn spring-boot:run
-Acesse o sistema em http://localhost:8080

Projeto desenvolvido para fins acadêmicos!!
