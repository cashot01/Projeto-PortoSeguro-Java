🚗 AutoCheckUP - Sistema de Diagnóstico Automotivo
AutoCheckUP é uma aplicação Java baseada em API REST que permite o gerenciamento de usuários, veículos e diagnósticos mecânicos. Foi projetada com arquitetura limpa, usando boas práticas de separação de camadas.

⚙️ Tecnologias Utilizadas:
- Java 11+
- JAX-RS (Jersey) – Para construção da API REST
- JPA (Jakarta Persistence) – Para persistência de dados
- Log4j – Para logs do sistema
- Maven – Para gerenciamento de dependências e build
- JUnit – Para testes


🔌 Funcionalidades da API
Usuários:

  - Criar, buscar, atualizar e deletar usuários

Veículos:

  - Cadastro de veículos com vínculo ao usuário (por CPF)

Diagnósticos:

   - Registro e recuperação de diagnósticos mecânicos

Login:

 - Endpoint para autenticação de usuários



🔧 Como Executar
1. Clone o repositório

  git clone https://github.com/seu-usuario/Projeto-PortoSeguro-Java.git
  cd Projeto-PortoSeguro-Java/AutoCheckUP-java

2. Compile o projeto

  mvn clean install
  
3. Execute a aplicação

  mvn exec:java -Dexec.mainClass="org.mecanica.Main"
  
A API será disponibilizada em: http://localhost:8080/api/

🧪 Rodando os Testes
  mvn test

📌 Endpoints de Exemplo:
Método	Endpoint	          Descrição
GET	      /usuarios	       Lista todos os usuários
POST	    /veiculos	       Cadastra um veículo
GET	      /diagnosticos	   Lista os diagnósticos
POST	    /login	         Realiza login do usuário


📚 Observações
O projeto está modularizado com repositórios genéricos para facilitar a manutenção e reuso.

A base de dados deve ser configurada dentro de DatabaseConfig.java
