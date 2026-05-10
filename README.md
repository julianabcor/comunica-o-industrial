🚀 Integração Vertical e Telemetria IIoT: Do Chão de Fábrica à Nuvem

Este projeto demonstra a implementação de uma arquitetura de **Indústria 4.0**, focada na integração vertical de dados. O objetivo é coletar dados de sensores simulados (temperatura e pressão) e transportá-los de forma segura e eficiente até plataformas de gestão e análise estratégica.

🔍 Visão Geral
O projeto elimina as "ilhas de automação" ao conectar o nível de campo (sensores) diretamente ao nível de gestão (BI). Utilizamos protocolos industriais e de IoT para garantir que a informação bruta seja transformada em indicadores de performance (KPIs) e suporte para manutenção preditiva.

---

🏗 Arquitetura do Projeto
A solução é dividida em 5 camadas fundamentais:

1.  **Aquisição:** O microcontrolador **ESP32** (emulado via Wokwi) atua como um Gateway de Borda, realizando a leitura de sensores em tempo real.
2.  **Transporte:** Utilização do protocolo **MQTT** e do broker **HiveMQ** para envio de mensagens JSON leves e assíncronas.
3.  **Operação (HMI):** Interface web desenvolvida em **HTML/JavaScript** que consome os dados via WebSockets para monitoramento instantâneo.
4.  **Integração:** Orquestração de dados via **Make.com**, automatizando o fluxo entre o broker e o armazenamento em nuvem.
5.  **Inteligência:** Dashboards no **Power BI** para análise histórica, cálculo de KPIs e monitoramento preditivo de ativos.

---

🛠 Tecnologias Utilizadas

- **Simulação:** [Wokwi](https://wokwi.com/) (ESP32)
- **Protocolos:** MQTT, Modbus RTU, PROFINET, WebSockets
- **Mensageria:** HiveMQ (Broker)
- **Front-end:** HTML5, CSS3, JavaScript
- **Automação:** Make.com
- **Análise de Dados:** Microsoft Power BI

---

✨ Funcionalidades
- **Monitoramento em Tempo Real:** Visualização dinâmica de temperatura e pressão.
- **Sistema de Alarmística:** Alertas visuais automáticos no dashboard caso a temperatura exceda **30°C**.
- **Análise Preditiva:** Histórico de dados que permite identificar tendências de falha antes que ocorram paradas não planejadas.
- **Integração Vertical Completa:** O dado percorre todos os níveis da pirâmide ISA-95.

---

🚀 Como Executar

1. Simulação do Hardware
- Acesse o projeto no [Wokwi].
- Inicie a simulação para começar a transmissão via MQTT.

2. Dashboard Operacional
- Abra o arquivo `index.html` em seu navegador.
- Certifique-se de que o tópico MQTT configurado no JS é o mesmo do ESP32.

3. Visualização de Dados
- O fluxo de dados será processado pelo Make.com e alimentará o dashboard no Power BI [Link do Dashboard se houver].

---

👥 **Equipe - Grupo 04** (SENAI CentroWEG)
- **Amanda Miranda**
- **Juliana Cordeiro**
- **Rafael Elias**

**Professor Orientador:** Fabiano da Silva Luiz  
**Ano:** 2026
