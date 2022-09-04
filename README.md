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

