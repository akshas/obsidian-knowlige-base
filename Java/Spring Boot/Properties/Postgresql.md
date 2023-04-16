spring.datasource.url=jdbc:postgresql://localhost:5432/cards  
spring.datasource.username=alex  
spring.datasource.password=12345  
spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect  
spring.datasource.driver-class-name=org.postgresql.Driver  
spring.liquibase.change-log=db/changelog/master-changelog.yml  
spring.jpa.hibernate.ddl-auto=update

пробелы в конце строк могут вызывать ошибку
если есть ошибка драйвера, то надо перезапустить gradle