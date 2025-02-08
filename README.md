# Simulador-sensor-DHT11-con-Python-y-MQTT-HiveMQ


Este repositorio contiene un script en Python que simula un sensor DHT11 y publica datos de temperatura y humedad en un broker MQTT usando HiveMQ.

📌 ¿Qué es MQTT?
MQTT (Message Queuing Telemetry Transport) es un protocolo de mensajería ligera diseñado para la comunicación entre dispositivos IoT (Internet of Things). 
Se basa en un modelo publicador/suscriptor donde:

    Los publicadores envían mensajes a un topic.
    Los suscriptores reciben los mensajes de un topic específico.
    Un broker MQTT (como HiveMQ, Mosquitto, EMQX) gestiona la comunicación.

"paho-mqtt" es una biblioteca de Python que permite comunicarse con un broker MQTT para publicar y suscribirse a mensajes en diferentes topics.



🛠 ¿Para qué sirve paho-mqtt?

La librería paho-mqtt permite:

    ✅ Conectarse a un broker MQTT.

    ✅ Publicar mensajes en un topic.

    ✅ Suscribirse a un topic para recibir mensajes en tiempo real.

    ✅ Configurar opciones avanzadas como seguridad (TLS/SSL, autenticación).


🚀 ¿Dónde se usa paho-mqtt?

    Internet de las cosas (IoT): Sensores, domótica, smart devices.
  
    Monitorización en tiempo real: Datos de clima, mediciones industriales.
  
    Automatización: Control de dispositivos remotos.

📌 Requisitos

Python 3.x

      Biblioteca paho-mqtt


Instala la biblioteca necesaria con:

      pip install paho-mqtt      


⚙️ Configuración y Uso

1️⃣ Clonar el repositorio

     git clone https://github.com/tu_usuario/mqtt-dht11-simulator.git
     cd mqtt-dht11-simulator

2️⃣ Ejecutar el script

    python simulador_dht11.py

El script publicará cada 2 segundos datos simulados en el broker MQTT.



🔍 Visualizar los Datos en Tiempo Real

    Puedes ver los datos enviados al broker MQTT usando el HiveMQ Web Client.

    Pasos para suscribirse:

    Abre el enlace del HiveMQ Web Client. ( https://www.hivemq.com/demos/websocket-client/ )

    Haz clic en "Connect" (usa la configuración por defecto).

    En la sección "Subscribe", ingresa el topic:  sensor/dht11 y haz clic en **"Subscribe"`.

    Verás los datos publicados en tiempo real.
![image](https://github.com/user-attachments/assets/f295bdbc-0cb1-4cf3-93a5-849ec0777424)

🛠 Posibles Mejoras

    Agregar soporte para usuario/contraseña en el broker MQTT.

    Implementar conexión segura (TLS/SSL).

    Permitir configurar el broker y topic mediante variables de entorno.
