# Local

### Acessar as propriedades de configuração Local

Tem que ser referente ao tipo do arquivo que está na pasta config

http://localhost:8888/application-dev/default;

http://localhost:8888/application-hml/default;

http://localhost:8888/application-qa/default;

http://localhost:8888/application-prod/default;

### Configurar application.yml

```
spring:
  application:
    name: spring-config-server
  profiles:
    active:
    - native
```


# Remoto GITHUB

### Acessar as propriedades de configuração Remota

Irá buscar no repositório do github que esta referenciado no application.yml

http://localhost:8888/greeting-service/default;

http://localhost:8888/greeting-service/dev;

http://localhost:8888/greeting-service/hml;

http://localhost:8888/greeting-service/prod;

### Configurar application.yml

```
spring:
  application:
    name: greeting-service
  cloud:
    config:
      server:
        git:
          uri: https://github.com/douglasdjf/spring-config-server
          #username: 
          #password: 
```
