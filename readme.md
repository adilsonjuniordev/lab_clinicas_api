# Lab Clinicas API - JSON Rest Server (Flutter Experience)

[![forthebadge](https://forthebadge.com/images/badges/made-with-flutter.svg)](http://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/powered-by-coffee.svg)](http://forthebadge.com)

[![MIT License](https://img.shields.io/badge/Flutter-3.16.9-blue)](https://docs.flutter.dev/release/release-notes)
[![MIT License](https://img.shields.io/badge/Dart-3.2.6-blue)](https://docs.flutter.dev/release/release-notes)

Projeto desenvolvido em 01/2024, utilizando o Dart, com o intuito de aprimorar os conhecimentos no framework, utilizando arquitetura orientada à package, através de um core que será reaproveitado nas plataformas mobile, web e desktop.

## Stack utilizada

**Mobile:** Flutter (SDK versão inicial: 3.16.9)

## Como utilizar

Esta API local, utiliza o package JSON Rest Server como ferramenta para simular um backend local. Para utilizar a API localmente, configure o arquivo "config.yaml". Abaixo segue um exemplo de configuração:

```yaml
name: Json Rest Server
port: 8080
host: 0.0.0.0
database: database.json

auth:
   jwtSecret: cwsMXDtuP447WZQ63nM4dWZ3RppyMl
   jwtExpire: 3600
   unauthorizedStatusCode: 401
   urlSkip:
      - /images:
         method: get
      - /users:
         method: post
      - /adm_users:
         method: post
      - /products:
         method: get
      - /products/{*}:
         method: get

```

Habilite o package do JSON Rest Server globalmente no seu ambiente, executando:

```bash
dart pub global activate json_rest_server
```

Depois, no diretório raiz do projeto, execute o seguindo comando para iniciar a API localmente:

```bash
jrs run
```

Qualquer dúvida, entre em contato que estarei disposto a auxiliá-lo!

## Desenvolvedor

### Adilson Junior

[![github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/adilsonjuniordev)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adilsonjuniordev/)
