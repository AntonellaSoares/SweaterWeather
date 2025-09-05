
# Levantamento de APIs para o Sistema de Sugestão de Looks com Base no Clima


## 1. API de Previsão do Tempo 
### OpenWeatherMap
- **URL:** [https://openweathermap.org/api](https://openweathermap.org/api)
- **Dados fornecidos:** Temperatura, sensação térmica, umidade, vento, previsão para horas/dias.
- **Plano gratuito:** 60 chamadas/minuto (com algumas limitações).
- **Formato de retorno:** JSON.
- **Vantagem:** Suporte global, fácil integração, boa documentação.

## 2. API de Geolocalização (opcional)
Para identificar a localização do usuário automaticamente:

### IP Geolocation API
- **URL:** [https://ipgeolocation.io/](https://ipgeolocation.io/)
- **Função:** Detecta cidade, país e coordenadas pelo IP.
- **Uso:** Permite mostrar clima sem que o usuário digite a cidade.

### HTML5 Geolocation API
- **Função:** Permite obter a localização exata (com permissão do usuário).
- **Custo:** Gratuita, nativa em navegadores.

## 3. API de Imagens (para ilustrar looks)

### Pexels API
- **URL:** [https://www.pexels.com/api/](https://www.pexels.com/api/)
- **Função:** Imagens gratuitas e livres de direitos autorais.


## Estratégia de Integração
- **OpenWeatherMap** para dados climáticos.
- **HTML5 Geolocation API** para localização automática do usuário.
- **Unsplash API** para imagens ilustrativas das sugestões de looks.
