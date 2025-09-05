
# Levantamento de APIs para o Sistema de Sugestão de Looks com Base no Clima

## 1. API de Previsão do Tempo

### OpenWeatherMap
- **URL:** [https://openweathermap.org/api](https://openweathermap.org/api)
- **Dados fornecidos:** Temperatura, sensação térmica, umidade, vento, previsão para horas/dias.
- **Plano gratuito:** 60 chamadas/minuto (com algumas limitações).
- **Formato de retorno:** JSON.
- **Vantagem:** Suporte global, fácil integração, boa documentação.

### WeatherAPI
- **URL:** [https://www.weatherapi.com/](https://www.weatherapi.com/)
- **Dados fornecidos:** Clima atual, previsão para até 10 dias, qualidade do ar.
- **Plano gratuito:** 1 milhão de requisições/mês.
- **Formato:** JSON ou XML.
- **Vantagem:** Informações detalhadas e confiáveis, inclui ícones prontos.

### AccuWeather API
- **URL:** [https://developer.accuweather.com/](https://developer.accuweather.com/)
- **Dados fornecidos:** Clima atual, previsão horária e diária.
- **Plano gratuito:** 50 requisições/dia.
- **Ideal para:** Previsões mais precisas, porém uso gratuito limitado.

### Tomorrow.io (antiga Climacell)
- **URL:** [https://www.tomorrow.io/](https://www.tomorrow.io/)
- **Dados fornecidos:** Previsões hiperlocais, poluição, alertas climáticos.
- **Plano gratuito:** 500 requisições/dia.
- **Ideal para:** Aplicações que exigem dados detalhados.

---

## 2. API de Geolocalização (opcional)
Para identificar a localização do usuário automaticamente:

### IP Geolocation API
- **URL:** [https://ipgeolocation.io/](https://ipgeolocation.io/)
- **Função:** Detecta cidade, país e coordenadas pelo IP.
- **Uso:** Permite mostrar clima sem que o usuário digite a cidade.

### HTML5 Geolocation API
- **Função:** Permite obter a localização exata (com permissão do usuário).
- **Custo:** Gratuita, nativa em navegadores.

---

## 3. API de Imagens (para ilustrar looks)
### Unsplash API
- **URL:** [https://unsplash.com/developers](https://unsplash.com/developers)
- **Função:** Fotos gratuitas e de alta qualidade.
- **Uso:** Ilustrar as sugestões de looks.

### Pexels API
- **URL:** [https://www.pexels.com/api/](https://www.pexels.com/api/)
- **Função:** Imagens gratuitas e livres de direitos autorais.

---

## Estratégia de Integração
- **OpenWeatherMap** para dados climáticos.
- **HTML5 Geolocation API** para localização automática do usuário.
- **Unsplash API** para imagens ilustrativas das sugestões de looks.

---

## Observação
As APIs fornecem os dados necessários, mas a lógica de sugestão de looks será desenvolvida no sistema, baseada nos dados meteorológicos retornados pela API.
levantamento_apis.md
Exibindo levantamento_apis.md.
