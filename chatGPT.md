## install chatGPT with docker-compose.yaml
```
version: '2'
networks:
  net1:
    driver: bridge
services:
  app:
    container_name: gpt
    image: chenzhaoyu94/chatgpt-web:main
    restart: always
    ports:
      - "8282:3002"
    environment:
      OPENAI_API_KEY: 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
      TIMEOUT_MS: 60000
```
