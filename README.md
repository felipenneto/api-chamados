# API de chamados de suporte

**Estudante** — Felipe Alves Bezerra Neto

## Objetivo

Criar a estrutura inicial de uma API de chamados de suporte com Flask, usando o uv para gerenciar o ambiente e as dependências. Nesta primeira etapa, a rota inicial informa se a API está em funcionamento.

## Instalação

Com o uv instalado, execute na pasta do projeto:

```bash
uv sync --locked
```

## Execução

```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

## Verificação

Abra [http://localhost:5000/](http://localhost:5000/). No GitHub Codespaces, abra a URL encaminhada para a porta 5000 na aba **Portas**. Para conferir a resposta pelo terminal, execute:

```bash
curl -i http://localhost:5000/
```

A rota `GET /` responde com o status HTTP `200 OK`, o cabeçalho `Content-Type: application/json` e o seguinte objeto JSON:

```json
{
  "mensagem": "API de chamados em funcionamento"
}
```
