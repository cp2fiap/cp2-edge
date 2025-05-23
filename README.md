Participantes: Azor Biagioni Tartuce RM 563995
Gabriel Viana de Sousa RM 564382

Link para simulação: https://wokwi.com/projects/431675152860634113

🍷 Sistema de Monitoramento para Vinheria - Arduino
📋 Descrição
Este projeto consiste em um sistema automatizado de monitoramento de temperatura, umidade, luminosidade e horário para uma vinheria, utilizando um Arduino e sensores diversos. O sistema exibe informações em tempo real em um display LCD e aciona LEDs e buzzer de acordo com condições ambientais pré-estabelecidas.

Além disso, realiza o registro de dados de temperatura e umidade na memória EEPROM, permitindo a recuperação posterior do histórico via comunicação serial.

🎯 Funcionalidades
✅ Monitoramento de temperatura e umidade com sensor DHT22
✅ Exibição de data e hora em tempo real com módulo RTC DS1307
✅ Exibição de informações no LCD I2C
✅ Controle de LEDs e buzzer conforme níveis de luminosidade detectados com sensor LDR
✅ Registro de logs na EEPROM para consulta posterior
✅ Ajuste automático do horário com compensação de fuso UTC -3

🛠️ Tecnologias e Componentes Utilizados
Arduino Uno/Nano

Sensor de temperatura e umidade DHT22

Módulo RTC DS1307

Display LCD I2C 16x2

Sensor de luminosidade LDR

LEDs verde, amarelo e vermelho

Buzzer

Memória EEPROM

Biblioteca LiquidCrystal_I2C

Biblioteca RTClib

Biblioteca DHT

⚡ Como Usar
Monte o circuito conforme a descrição:

DHT22 no pino digital 2

LEDs e buzzer nos pinos digitais 8, 9, 10 e 11

LDR ligado ao pino analógico A0

Módulo RTC DS1307 conectado via I2C (padrão: SDA e SCL)

Display LCD via I2C (endereço 0x27 ou 0x3F, conforme o modelo)

Carregue o código no Arduino usando a IDE Arduino.

Ajuste o relógio na primeira vez
RTC.adjust(DateTime(2025, 5, 22, 13, 39, 0));


<img width="1320" alt="Captura de Tela 2025-05-23 às 19 04 22" src="https://github.com/user-attachments/assets/53513153-2963-44fa-8f05-fd134a10cf8f" />
