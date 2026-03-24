# Automacao_N8N_APIs_Telegram
A#  Telegram Automation Bot com n8n

Automação de processos via Telegram utilizando **n8n** com integração a APIs externas como **Google Drive**, **Google Docs** e consumo de **feeds RSS**.

Este projeto demonstra a construção de um chatbot funcional capaz de gerar documentos automaticamente, manipular conteúdo dinâmico e fornecer informações em tempo real.

---

##  Funcionalidades

###  Caso 1 — Geração automática de documentos

* Criação de documentos no Google Docs a partir de texto enviado via Telegram
* Substituição dinâmica de conteúdo
* Exportação automática para PDF
* Geração de link público para compartilhamento

---

### Caso 2 — Documento com texto + imagem dinâmica

* Uso de marcadores personalizados (placeholders)
* Inserção dinâmica de texto e imagem
* Upload de arquivos via Telegram
* Integração com Google Drive para manipulação de arquivos
* Geração automática de documentos personalizados

---

###  Caso 3 — Bot de notícias (G1)

* Consumo de feed RSS
* Extração de títulos e links
* Envio formatado das principais notícias via Telegram

---

##  Integrações / APIs utilizadas

* Telegram Bot API
* Google Drive API
* Google Docs API
* RSS Feed (G1)
* HTTP Request (integrações REST)

---

##  Tecnologias utilizadas

* n8n (automação low-code)
* Webhooks
* APIs REST
* JSON
* Google Cloud Platform

---

##  Fluxo da aplicação

1. Usuário interage com o bot no Telegram
2. Webhook do Telegram aciona o n8n
3. O workflow identifica o comando enviado
4. Executa integrações com APIs externas
5. Processa os dados dinamicamente
6. Retorna o resultado ao usuário no Telegram

---

## 📸 Demonstração



### 🔧 Workflow no n8n

![Workflow](images/fluxo.png)

### 💬 Bot no Telegram

![Bot](images/bot.png)

### 📄 Documento gerado

![Documento](images/documento.png)

---

##  Estrutura do projeto

```
telegram-n8n-automation/
│
├── workflow.json
├── README.md
└── images/
    ├── fluxo.png
    ├── bot.png
    └── documento.png
```

---

## ⚡ Como usar

1. Clone o repositório:

```
git clone https://github.com/seu-usuario/telegram-n8n-automation.git
```

2. Importe o arquivo `workflow.json` no n8n

3. Configure as credenciais:

   * Telegram Bot
   * Google Drive / Docs (OAuth2)
   * Permissões de compartilhamento de arquivos

4. Ative o workflow

5. Inicie o bot no Telegram com:

```
/start
```

---

##  Destaques técnicos

* Automação completa baseada em eventos (webhooks)
* Integração com múltiplas APIs externas
* Geração dinâmica de documentos
* Manipulação de arquivos (upload, download, compartilhamento)
* Estrutura modular de workflow no n8n

---




