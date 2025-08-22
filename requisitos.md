# Documento de Requisitos – Sweater Weather API

---

## Requisitos Funcionais (RF)

- **RF01 – Integração com API de Previsão do Tempo**  
  O sistema deve consultar uma API de clima em tempo real para obter dados atualizados sobre as condições meteorológicas (temperatura, sensação térmica, umidade, velocidade do vento, etc.).  
  ➝ A API deve ser consultada sempre que o usuário acessar a aplicação para garantir informações atualizadas.  

- **RF02 – Sugestão de Looks Baseada nas Condições Climáticas**  
  O sistema deve sugerir combinações de roupas com base nas condições meteorológicas.  
  ➝ Exemplo: se estiver frio, sugerir agasalhos como cardigã e calça jeans; se estiver quente, sugerir roupas leves como shorts e regatas.  

- **RF03 – Exibição da Previsão do Tempo da localidade**  
  O sistema deve exibir a previsão do tempo atual e futura do local desejado de maneira clara, incluindo:  
  - Temperatura atual.  
  - Sensação térmica.  
  - Probabilidade de chuva.  
  - Condições gerais (ensolarado, nublado, chuvoso, etc.).  
  - Projeção do tempo para o restante do dia.  

- **RF04 – Sugestões de Roupas e Tecidos**  
  As sugestões de looks devem considerar tipos de tecidos adequados **e também tecidos a evitar**, conforme o clima:  

  - **Clima quente**:  
    - Usar: algodão, linho, viscose.  
    - Evitar: poliéster pesado, lã, couro.  

  - **Clima frio**:  
    - Usar: lã, flanela, tricô, fleece.  
    - Evitar: linho e seda.  

  - **Chuva/neve**:  
    - Usar: nylon, poliéster tratado, couro sintético, tecidos impermeáveis.  
    - Evitar: algodão e jeans.  

  - **Vento forte**:  
    - Usar: softshell, poliéster encorpado, corta-vento.  
    - Evitar: seda e malha leve.  

  - **Clima úmido**:  
    - Usar: dry-fit, poliamida, tecidos respiráveis de secagem rápida.  
    - Evitar: veludo, lã grossa, jeans pesado.  

- **RF05 – Categorias de Look**  
  O sistema deve permitir que os looks sejam sugeridos por categorias, como “lazer”, “trabalho” e “esporte”.  

- **RF06 – Tela de Resultado**  
  A tela principal deve mostrar a previsão do tempo atual e as sugestões de looks para o dia de forma clara e visualmente atraente.  
  ➝ A sugestão de roupas deve vir acompanhada de uma breve explicação sobre como se adapta às condições climáticas.  

---

## Requisitos Não Funcionais (RNF)

- **RNF01 – Desempenho**  
  O tempo de resposta da aplicação deve ser inferior a 2 segundos nas consultas à API de clima.  
  A aplicação deve carregar rapidamente em dispositivos móveis e desktop.  

- **RNF02 – Escalabilidade**  
  O sistema deve suportar múltiplos usuários simultâneos sem perda de performance.  

- **RNF03 – Segurança**  
  Todas as requisições à API de clima devem ser feitas via HTTPS.  
  O sistema não deve apresentar vulnerabilidades comuns (XSS, CSRF, etc.).  

- **RNF04 – Usabilidade**  
  A interface deve ser simples, intuitiva e clara.  
  ➝ A visualização das roupas sugeridas deve ser visualmente atraente.  
  ➝ O design deve ser responsivo, adequado a mobile e desktop.  

- **RNF05 – Compatibilidade**  
  O sistema deve funcionar nos principais navegadores modernos (Chrome, Firefox, Safari, Edge).  

- **RNF06 – Manutenibilidade**  
  O código deve ser bem estruturado, documentado e seguir boas práticas para facilitar futuras manutenções.  

- **RNF07 – Alta Disponibilidade**  
  A aplicação deve estar disponível 24/7, com mínima indisponibilidade.  
  ➝ Em caso de falha na API de clima, o sistema deve exibir mensagem amigável ao usuário.  

- **RNF08 – Internacionalização**  
  O sistema deve permitir escolha de unidades (Celsius/Fahrenheit, km/h, mph).  
  A interface deve estar preparada para tradução em outros idiomas.  

- **RNF09 – Acessibilidade**  
  O sistema deve seguir diretrizes WCAG para garantir acessibilidade a usuários com deficiência.  

- **RNF10 – Consumo de API**  
  O sistema deve otimizar as chamadas à API de clima, evitando excesso de requisições e garantindo bom desempenho.  

---
