# Avaliacoes-M7-Inteli

Avaliações do Módulo 7

Para executar o backend:

```bash
python main.py
```

Para executar o frontend:

```bash
node server.js
```

| **_IMPORTANTE:_** Utilizar dentro do contexto do container.

## Adições do betinho

Para iniciar o código na root rode:

```bash
docker compose up
```

Para entrar no frontend (muito "bonito" e "funcional") rode va até <http://localhost:3000>

## decisões nos dockerfiles

O docker file do backend começa copaindo todos os arquivos e rodando um install dos requirements após isso rodamos o servidor com o commando "uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000".
O docker file do frontend começa copiando os arquivos e dando um npm install para baixar dependências após isso rodamos o servidor com "node","server.js"
O docker compose simplemente aloca as portas certas a cada aplicação e pega as imagens do dockerhub
