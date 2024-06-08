# Sistema de Fila com Apache Kafka

Este documento fornece instruções básicas para instalar, configurar e operar o sistema de fila desenvolvido com Apache Kafka e Docker.

## Instalação

#### Pré-requisitos:

- Docker
- Clone o repositório do projeto.
-  Navegue até o diretório do projeto.

## Configuração

- O sistema utiliza Docker Compose.
- O arquivo `docker-compose.yml` está configurado e pronto para uso.

## Operação

1. **Inicialização:**
   ```bash
   docker-compose up
   ```
2. **Uso:**
   - O produtor recebe requisições POST em `http://localhost:8080`.
   - O consumidor processa mensagens automaticamente.
3. **Encerramento:**
   Pressione `Ctrl + C`.

#### Exemplo de requisição:
  
```json
{
  "message": "Sua mensagem" 
}
```
### Exemplo de Resposta

```json
{
    "message": "Mensagem enviada para o Kafka"
}
```
