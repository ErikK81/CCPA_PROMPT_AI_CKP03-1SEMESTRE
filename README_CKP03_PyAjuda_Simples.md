# PyAjuda — Chatbot de Dúvidas de Python

**CKP03 — Chatbot Especializado | FIAP**

**Integrantes:** Erik Criscuolo/RM574565.

## Sobre o projeto

O **PyAjuda** é um chatbot simples que ajuda iniciantes a aprender Python. Ele explica conceitos básicos, mostra exemplos curtos e responde dúvidas sobre erros de código.

O chatbot usa o modelo gratuito `gpt-oss:120b` pela Ollama Cloud e foi feito para rodar no Google Colab.

## Funcionalidades

- Responde perguntas sobre Python em português simples.
- Mantém o histórico da conversa para entender perguntas seguintes.
- Usa uma persona de professor paciente, definida no *system prompt*.
- Recusa educadamente perguntas que não sejam sobre Python.
- Mostra três conversas de exemplo com três perguntas cada.

## Exemplos de uso

O notebook executa automaticamente três situações:

| Situação | O que é testado |
|---|---|
| Caso normal | Listas, adicionar elementos e acessar o primeiro item |
| Caso difícil | Divisão por zero, `try/except` e continuidade da conversa |
| Fora do escopo | Pergunta sobre futebol, explicação do domínio do bot e retorno a Python |

Cada situação possui três perguntas consecutivas. As respostas são geradas pela IA durante a execução e podem variar.

## Tecnologias

- Python
- Google Colab
- Biblioteca `requests`
- Ollama Cloud (`gpt-oss:120b`)