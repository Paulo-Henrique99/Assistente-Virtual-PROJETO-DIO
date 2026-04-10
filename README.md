# 💰 FinAssist AI

Assistente financeiro inteligente desenvolvido com **Python, Flask e Google Gemini AI**, capaz de responder perguntas sobre finanças utilizando FAQ, cálculos automáticos e inteligência artificial.

---

## 🚀 Tecnologias

- Python 3
- Flask
- Google Gemini API
- HTML / CSS / JavaScript

---

## ⚙️ Funcionalidades

- Respostas rápidas via FAQ
- Simulações financeiras automáticas
- Integração com IA (Gemini)
- Histórico de contexto em conversa
- Tratamento de erros da API

---

## 📂 Estrutura do Projeto

```bash
finassist-ai/
│
├── app.py
├── core/
│   ├── ai.py
│   ├── faq.py
│   └── calc.py
│
├── templates/
├── static/
├── .env
└── requirements.txt
```

---

## 🔐 Configuração

Crie um arquivo `.env` na raiz:

```env
GEMINI_API_KEY=sua_chave_aqui
```

---

## ▶️ Como Executar

```bash
# Criar ambiente virtual
python -m venv .venv

# Ativar ambiente
.venv\Scripts\activate

# Instalar dependências
pip install -r requirements.txt

# Rodar projeto
python app.py
```

Aplicação disponível em:

```bash
http://127.0.0.1:5000
```

---

## 📡 Endpoint Principal

### POST `/chat`

```json
{
  "message": "qual melhor investimento?"
}
```

---

## 👨‍💻 Autor

Desenvolvido por **Paul Henrique**

Projeto criado para estudo, prática e portfólio.
