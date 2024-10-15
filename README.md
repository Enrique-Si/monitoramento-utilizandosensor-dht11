Projeto IoT: Monitoramento de Temperatura e Umidade com Sensor DHT11 e ESP32

Este projeto foi desenvolvido com o objetivo de criar um sistema de monitoramento de temperatura e umidade utilizando o sensor DHT11 conectado a um microcontrolador ESP32. O sistema coleta os dados ambientais e os transmite para a plataforma ThingSpeak, que permite o armazenamento e visualização desses dados em tempo real.

Funcionalidades 📊

	•	Leitura de Temperatura e Umidade: O sensor DHT11 coleta os dados de temperatura e umidade do ambiente a cada 5 segundos.
	•	Envio de Dados para ThingSpeak: Os dados são enviados automaticamente para a plataforma ThingSpeak através de uma conexão Wi-Fi, permitindo o monitoramento remoto.
	•	Controle de Relé: Caso a temperatura ultrapasse 31°C ou a umidade esteja acima de 70%, um relé é ativado automaticamente, permitindo o controle de um dispositivo externo (como um ventilador ou ar-condicionado).

Tecnologias Utilizadas 🛠️

	•	Python: Linguagem utilizada para o desenvolvimento do código no ESP32.
	•	DHT11: Sensor de temperatura e umidade.
	•	ESP32: Microcontrolador que processa os dados e realiza a conexão Wi-Fi.
	•	ThingSpeak: Plataforma para visualização e monitoramento dos dados coletados.

Como Funciona 🔧

	1.	O sensor DHT11 coleta os dados de temperatura e umidade do ambiente.
	2.	Os dados são enviados para a plataforma ThingSpeak usando uma conexão Wi-Fi configurada no ESP32.
	3.	Se a temperatura for maior que 31°C ou a umidade maior que 70%, o relé é acionado para controlar um dispositivo de resfriamento, como um ventilador.
	4.	Caso contrário, o relé permanece desligado.

Instruções de Uso 🚀

	1.	Conecte o sensor DHT11 ao ESP32 utilizando os pinos apropriados.
	2.	Configure sua rede Wi-Fi no código, substituindo o SSID e senha pela sua rede local.
	3.	Insira sua chave API do ThingSpeak para que os dados sejam enviados corretamente.
	4.	Suba o código no ESP32 utilizando o Thonny ou outra IDE de sua escolha.
	5.	Acesse a plataforma ThingSpeak para visualizar os dados em tempo real.

Estrutura do Código 📂

	•	wifi_lib.py: Responsável pela configuração da conexão Wi-Fi do ESP32.
	•	main.py: Código principal que realiza a leitura dos dados do sensor, controle do relé e envio dos dados para o ThingSpeak.

Requisitos

	•	ESP32
	•	Sensor DHT11
	•	Conta na plataforma ThingSpeak
	•	IDE Thonny (ou qualquer outra que suporte desenvolvimento em Python para ESP32)
