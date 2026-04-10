# 💰 FinAssist AI

Assistente financeiro inteligente desenvolvido com **Python + Flask + Gemini AI**, capaz de responder perguntas sobre finanças utilizando:

- 📚 Base de FAQ personalizada
- 🧮 Simulações financeiras automáticas
- 🤖 Inteligência Artificial com Google Gemini
- 🧠 Contexto de conversa para respostas mais naturais

---

# 🚀 Tecnologias Utilizadas

- Python 3.14
- Flask
- Google Gemini API
- HTML/CSS/JavaScript
- JSON
- Virtual Environment (venv)

---

# 📂 Estrutura do Projeto

```bash
finassist-ai/
│
├── app.py
│
├── core/
│   ├── ai.py
│   ├── faq.py
│   └── calc.py
│
├── templates/
│   └── index.html
│
├── static/
│   ├── style.css
│   └── script.js
│
├── .env
│
├── requirements.txt
│
└── README.md
```

---

# ⚙️ Funcionalidades

## 📚 FAQ Inteligente
O sistema verifica primeiro se a pergunta do usuário está cadastrada em uma base de respostas rápidas.

Exemplo:

- "o que é cdi?"
- "o que é selic?"
- "como funciona investimento?"

---

## 🧮 Simulação Financeira
Caso a mensagem contenha termos financeiros/calculáveis, o sistema tenta gerar uma simulação.

Exemplo:

- "simule rendimento de 1000 reais"
- "quanto rende 5000 por mês"

---

## 🤖 Integração com IA (Gemini)
Se não houver resposta no FAQ ou cálculo, a pergunta é enviada para o modelo Gemini para resposta dinâmica.

---

## 🧠 Memória de Conversa
O bot mantém contexto das últimas mensagens para tornar a conversa mais natural.

---

# 🔐 Configuração da API Key

Crie um arquivo `.env` na raiz do projeto:

```env
GEMINI_API_KEY=sua_chave_aqui
```

---

# 📦 Instalação do Projeto

## 1. Clone o repositório

```bash
git clone https://github.com/seuusuario/finassist-ai.git
```

---

## 2. Entre na pasta

```bash
cd finassist-ai
```

---

## 3. Crie ambiente virtual

```bash
python -m venv .venv
```

---

## 4. Ative ambiente virtual

### Windows:

```bash
.venv\Scripts\activate
```

### Linux/Mac:

```bash
source .venv/bin/activate
```

---

## 5. Instale dependências

```bash
pip install -r requirements.txt
```

---

# ▶️ Executando o Projeto

```bash
python app.py
```

Servidor iniciará em:

```bash
http://127.0.0.1:5000
```

---

# 🔄 Rotas da API

## Home

### GET `/`

Retorna status da aplicação:

```json
🚀 Finance AI com Gemini rodando com sucesso!
```

---

## Chat

### POST `/chat`

### Body:

```json
{
  "message": "qual melhor investimento?"
}
```

---

### Resposta:

```json
{
  "response": "Depende do seu perfil de investidor..."
}
```

---

# 🛡️ Tratamento de Erros

O projeto possui tratamento de falhas para:

- Quota excedida da API Gemini
- Erros de conexão externa
- Falhas internas do servidor
- Requisições inválidas

Caso a IA esteja indisponível:

```json
{
  "response": "⚠️ IA temporariamente indisponível no momento."
}
```

---

# 🧠 Fluxo de Funcionamento

O backend segue esta lógica:

```text
Usuário envia mensagem
       ↓
Verifica FAQ
       ↓
Se não encontrar:
Verifica Simulação Financeira
       ↓
Se não encontrar:
Consulta Gemini AI
       ↓
Retorna resposta ao usuário
```

---

# 📈 Melhorias Futuras

- Login de usuários
- Banco de dados para histórico permanente
- Dashboard financeiro
- Upload de planilhas
- Recomendações personalizadas de investimento
- Integração com APIs financeiras reais

---

# 👨‍💻 Autor

Desenvolvido por **Paulo Henrique Alves da Silva**

📌 Projeto criado para fins de estudo, portfólio e evolução profissional.

---

# ⭐ Licença

Este projeto está sob licença MIT.

Sinta-se livre para estudar, modificar e utilizar.