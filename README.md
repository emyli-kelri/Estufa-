# Mini-Estufa Automatizada

Projeto acadêmico desenvolvido para **monitoramento e controle das condições ambientais** de uma estufa em formato de casinha.  
O sistema utiliza um **ESP32** para realizar leituras de sensores, processar informações e acionar atuadores conforme necessário.  
Os dados podem ser exibidos em tempo real no **Blynk** ou enviados via **MQTT** para armazenamento e análise.

---

## Funcionalidades

- Monitoramento de:
  - Temperatura do ar; 
  - Umidade do ar; 
  - Luminosidade;  
  - Umidade do solo.  

- Controle automatizado de:
  - Ventilação (ventoinhas); 
  - Iluminação (LEDs). 

- Envio de dados para:
  - Plataforma **Blynk**;  
  - Servidor **MQTT**. 

- Visualização em tempo real no **monitor serial**.

---

## Componentes Utilizados

- **ESP32**. 
- **Sensores:**
  - DHT11 → Temperatura e umidade do ar; 
  - BH1750 → Luminosidade;  
  - Sensor de umidade do solo. 
- **Atuadores:**
  - Ventoinhas;  
  - LEDs.  
- **Conexão e comunicação:**
  - Wi-Fi integrado ao ESP32; 
  - Blynk (app de IoT);  
  - Mosquitto MQTT Broker.  

---

## Lógica de Funcionamento

- O **ESP32** realiza leituras periódicas dos sensores;  
- Se a temperatura ultrapassar o limite → ventoinhas são acionadas;  
- Se a luminosidade estiver abaixo do limite → LEDs são ligados.  
- Dados enviados para:
  - **Blynk** (monitoramento remoto via app);  
  - **MQTT** (monitoramento remoto via dashboards).  

---



