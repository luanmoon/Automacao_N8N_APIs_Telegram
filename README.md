# Automacao_N8N_APIs_Telegram
#  Telegram Automation Bot com n8n

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

##  Demonstração



###  Workflow no n8n

<img width="1667" height="581" alt="workflow" src="https://github.com/user-attachments/assets/262975d1-c597-4a6c-a94f-ba4feba69a1f" />


###  Bot no Telegram

Exemplo caso 1:
<img width="637" height="753" alt="bot 1" src="https://github.com/user-attachments/assets/05605a83-f7f4-4d0b-af33-9e90b569762f" />
<img width="576" height="449" alt="image" src="https://github.com/user-attachments/assets/91c4fff9-f47c-4110-81c3-e92e7ef5c784" />

Exemplo caso 2:
<img width="643" height="681" alt="bot 2" src="https://github.com/user-attachments/assets/79a86e95-7bb5-4b47-b7c8-be80a23f66a8" />

Exemplo caso 3:
<img width="649" height="754" alt="bot 3" src="https://github.com/user-attachments/assets/abab80ec-b60d-4e48-82a0-95bb8b5dee64" />
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

##  Como usar

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




