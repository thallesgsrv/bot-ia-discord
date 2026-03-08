# Discord AI Bot

Bot para **Discord** que utiliza um modelo de IA rodando localmente através do **Ollama**.

O bot permite fazer perguntas para a IA e encontrar **recursos gratuitos de estudo** sobre programação.

---

# Funcionalidades

## /ai

Envia uma pergunta para a IA e recebe uma resposta gerada pelo modelo local.

Exemplo:

```
/ai prompt: explique o algoritmo quicksort
```

---

## /recursos

Busca links gratuitos para estudar um determinado tema.

Exemplo:

```
/recursos termo: estruturas de dados
```

O comando retorna links de plataformas como:

- Dev.to
- freeCodeCamp
- GeeksForGeeks
- Anna's Archive
- Library Genesis

---

# Tecnologias utilizadas

- Python
- discord.py
- python-dotenv
- Ollama
- WizardCoder

---

# Requisitos

Antes de rodar o bot, instale:

- Python **3.9+**
- Ollama

---

# Instalar dependências Python

Clone o repositório e instale as dependências:

```bash
pip install -r requirements.txt
```

---

# Instalar Ollama

Instale o Ollama:

https://ollama.com

---

# Baixar o modelo utilizado

O bot usa o modelo **WizardCoder**.

Execute:

```bash
ollama pull wizardcoder
```

---

# Configuração

Crie um arquivo `.env` na raiz do projeto:

```
DISCORD_TOKEN=seu_token_aqui
```

O token pode ser obtido criando um bot no **Discord Developer Portal**.

---

# Configurar canal permitido

No código existe a variável:

```python
CANAL_ID = 1423834073776001075
```

Substitua pelo **ID do canal onde os comandos poderão ser usados**.

---

# Executar o bot

Execute:

```bash
python bot.py
```

Se tudo estiver correto, aparecerá no terminal:

```
[LOG] Bot online — Slash commands sincronizados!
```

---

# Estrutura do projeto

```
project/
│
├── bot.py
├── requirements.txt
├── README.md
├── .env
│
├── __pycache__/
└── .idea/
```

---

# Observações

- O bot precisa que o **Ollama esteja instalado e funcionando**.
- O modelo **wizardcoder** deve estar instalado.
- O bot só responde no canal configurado em `CANAL_ID`.

---

# Licença

Projeto aberto para estudo e experimentação.
