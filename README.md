Telegram Weather Bot ☀️

Bot de Telegram desenvolvido com n8n e OpenWeather API.

Funcionalidades

* Recebe o nome de uma cidade pelo Telegram
* Consulta a API OpenWeather
* Retorna:
    * Temperatura
    * Sensação térmica
    * Clima
    * Umidade
    * Velocidade do vento

Tecnologias

* n8n
* Telegram Bot API
* OpenWeather API

Fluxo

Telegram Trigger
↓
HTTP Request (OpenWeather)
↓
Edit Fields
↓
Send Telegram

Exemplo

Usuário:

Paris

Bot:

🌡️ Temperatura: 24°C
🤔 Sensação térmica: 26°C
☁️ Clima: céu limpo
💧 Umidade: 55%
💨 Vento: 12 km/h

Como usar

1. Crie um bot com o BotFather
2. Gere uma API Key no OpenWeather
3. Importe o arquivo workflow.json no n8n
4. Configure as credenciais do Telegram
5. Ative o workflow

Autor
Thaís Sgalbiero
