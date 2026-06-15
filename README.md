# 🌡️ Telegram Weather Bot com N8N

Bot do Telegram desenvolvido utilizando N8N que consulta a temperatura atual de qualquer cidade do Brasil.

## Tecnologias

- N8N
- Telegram Bot API
- OpenWeatherMap API

## Funcionalidades

- Consulta temperatura atual
- Sensação térmica
- Umidade
- Velocidade do vento
- Condições climáticas

## Configuração

### 1. Criar Bot Telegram

Fale com @BotFather e gere um token.

### 2. Criar API Key

https://openweathermap.org/api

### 3. Configurar N8N

Importe o workflow:

```text
workflow/telegram-weather-bot.json
```

### 4. Atualizar credenciais

Substitua:

```text
SEU_TOKEN_TELEGRAM
SUA_API_KEY
```

pelos valores corretos.

## Exemplo

Usuário:

```text
Rio de Janeiro
```

Bot:

```text
🌡️ Temperatura: 28°C

🤔 Sensação térmica: 31°C

☁️ Clima: Céu limpo

💧 Umidade: 68%

💨 Vento: 12 km/h
```

## Demonstração

### Workflow

![Workflow](screenshots/workflow.png)

### Exemplo Telegram

![Telegram](screenshots/telegram-example.png)

## Autor

Thaís Sgalbiero
