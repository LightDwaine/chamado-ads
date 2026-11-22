# API de Chamados de Suporte

**Estudante:** Jonathan Oliveira Silva

## Objetivo do Projeto
Desenvolver a estrutura inicial de uma API REST para gerenciamento de chamados de suporte utilizando Python e Flask, com gerenciamento de ambiente e dependências realizado pelo `uv`.

## Instalação das Dependências
Com o `uv` instalado, execute o comando abaixo na raiz do projeto para sincronizar o ambiente virtual com as versões exatas travadas no `uv.lock`:

```bash
uv sync --locked
```

## Execução da Aplicação
Para iniciar o servidor Flask (inclusive em ambientes como GitHub Codespaces), execute:

```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

## Como Acessar e Resposta Esperada
Com a aplicação em execução, faça uma requisição `GET` para a rota inicial:

- **URL:** `http://localhost:5000/`
- **Teste via terminal:**
  ```bash
  curl -i http://localhost:5000/
  ```
- **Status HTTP esperado:** `200 OK`
- **Cabeçalho:** `Content-Type: application/json`
- **Corpo da resposta (JSON):**
  ```json
  {
    "mensagem": "API de chamados em funcionamento"
  }
  ```