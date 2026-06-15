# 🌡️ Telegram Weather Bot com N8N

Um chatbot no Telegram desenvolvido com **N8N** que informa a temperatura atual de qualquer cidade do Brasil utilizando uma API de clima em tempo real.

## 📋 Sobre o desafio

Neste desafio, foi desenvolvido um chatbot integrado ao Telegram capaz de receber o nome de uma cidade brasileira e retornar informações meteorológicas atualizadas, incluindo:

* Temperatura atual
* Sensação térmica
* Condição climática
* Umidade do ar
* Velocidade do vento

Toda a automação foi construída utilizando o N8N, sem necessidade de desenvolvimento backend tradicional.

---

## 🚀 Tecnologias utilizadas

* N8N
* Telegram Bot API
* OpenWeatherMap API
* Webhooks
* JSON

---

## 📂 Estrutura do Projeto

```
telegram-weather-bot/
│
├── workflow/
│   └── telegram-weather-bot.json
│
├── screenshots/
│   ├── workflow.png
│   ├── telegram-example.png
│
├── README.md
└── .env.example
```

---

## ⚙️ Como funciona

1. O usuário envia uma mensagem para o bot no Telegram.
2. O Telegram envia o evento para o N8N.
3. O workflow captura o nome da cidade.
4. O N8N consulta a API OpenWeatherMap.
5. Os dados meteorológicos são processados.
6. O bot responde ao usuário com as informações climáticas.

---

## 🔧 Configuração

### 1. Criar um Bot no Telegram

Converse com o BotFather:

```
/newbot
```

Copie o token gerado.

---

### 2. Criar conta no OpenWeatherMap

Acesse:

https://openweathermap.org/api

Gere sua API Key gratuita.

---

### 3. Configurar variáveis

Crie um arquivo `.env`:

```env
TELEGRAM_TOKEN=seu_token
OPENWEATHER_API_KEY=sua_api_key
```

---

## 🔄 Workflow N8N

### Nó 1 — Telegram Trigger

Recebe mensagens do usuário.

### Nó 2 — HTTP Request

Consulta:

```http
https://api.openweathermap.org/data/2.5/weather?q={{cidade}},BR&appid={{API_KEY}}&units=metric&lang=pt_br
```

### Nó 3 — Set

Formata a resposta:

```text
🌡️ Temperatura: 25°C

🤔 Sensação térmica: 27°C

☁️ Clima: Céu limpo

💧 Umidade: 65%

💨 Vento: 10 km/h
```

### Nó 4 — Telegram

Envia a mensagem ao usuário.

---

## 💬 Exemplo de uso

Usuário:

```
São Paulo
```

Bot:

```text
🌡️ Temperatura: 22°C

🤔 Sensação térmica: 24°C

☁️ Clima: Nublado

💧 Umidade: 71%

💨 Vento: 8 km/h
```

---

## 🎯 Possíveis melhorias

* Previsão para os próximos 7 dias
* Geolocalização automática
* Consulta por CEP
* Cache de consultas
* Alertas meteorológicos
* Integração com WhatsApp

---

## 📸 Demonstração

Adicione aqui imagens do workflow e do funcionamento do bot.

---

## 👩‍💻 Autor

Desenvolvido por Thaís Sgalbiero durante o desafio de automação com N8N.

