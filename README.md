# Guia para Rodar o Backend da Aplicação de Imobiliária

## Integrantes do Projeto
- Vinicius de Carvalho Salvador
- Leonardo Henrique Florencio Cata Preta

## Pré-requisitos
Certifique-se de ter instalado em sua máquina:
- Java JDK 11 ou superior
- Maven 3.6 ou superior
- Banco de Dados (MySQL/PostgreSQL conforme configurado)

### Como verificar as instalações:

java -version
mvn -v

2. Configurar Variáveis de Ambiente

// trocar por banco local

spring.datasource.url=jdbc:mysql://localhost:3306/imobiliaria_db 
spring.datasource.username=imobiliaria_user
spring.datasource.password=senha_segura
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
server.port=8080

mvn clean install

3. Compilar o Projeto

mvn compile

4. Executar a Aplicação

mvn spring-boot:run
