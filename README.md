
# Creación del Chatbot Oficial del Hotel Costa Azul
> [!tip]
> #### Manual
> Ver [[Crear Chatbot.pdf|Crear Chatbot]]

El **Hotel CostaAzul**, un hotel de 4 estrellas situado en la costa mediterránea, quiere incorporar en su página web y en su aplicación móvil un **chatbot inteligente** que atienda a los clientes de forma automática antes, durante y después de su estancia.
## El chatbot deberá ayudar a los usuarios a:
- Consultar **disponibilidad de habitaciones**.
- Obtener información sobre **precios, servicios y horarios del hotel**.
- Realizar **preguntas frecuentes** (wifi, parking, restaurante, piscina…).
- Solicitar **asistencia inmediata** o ser derivados a un recepcionista humano.
- Recibir **recomendaciones personalizadas** sobre actividades locales.
## Funcionalidades mínimas del chatbot del hotel
### Saludo e identificación
El chatbot debe:
- Saludar al usuario.
- Presentarse como asistente del hotel (nombre del hotel).
- Preguntar en qué puede ayudar.
### Preguntas frecuentes (FAQ) del hotel  
El chatbot debe responder, como mínimo, a:
- Horario de **check-in** y **check-out**.
- Si hay **parking**, si es gratis o de pago.
- Disponibilidad de **wifi** y si tiene coste.
- Horario del **desayuno** y del restaurante.
- Si se aceptan **mascotas**.
- Servicios principales: piscina, spa, gimnasio, etc.
### Información básica de habitaciones
- Tipos de habitación (ej.: estándar, suite, familiar).
- Capacidad (nº de personas).
- Si incluyen desayuno o no.
- Política básica de cancelación (muy resumida).

No hace falta que haga una reserva real, pero debe **explicar opciones** cuando el usuario pregunte por habitaciones.
### Recomendaciones locales
El chatbot debe poder sugerir:
- **lugares turísticos** cercanos.
- restaurantes o actividades típicas (playa, rutas, etc.).

Responder a cosas del estilo:
- “¿Qué puedo hacer por la tarde cerca del hotel?”
- “¿Alguna recomendación para cenar?”
### Derivación a personal humano
El chatbot debe tener siempre una opción del tipo:
- “Hablar con recepción”
- “Quiero hablar con una persona”

Al activarla, debe:
- Mostrar un mensaje indicando que se pasa a un humano.
- Simular algún método de contacto: por ejemplo:
	- Mostrar el teléfono del hotel.
	- Mostrar un mensaje tipo “Un recepcionista te contestará por chat en unos minutos” (aunque no haya backend real).
### Gestión de errores / No entiendo
Si el chatbot no reconoce la pregunta:
- Mostrar un mensaje tipo “Lo siento, no he entendido tu pregunta”.
- Ofrecer opciones:
	- “Preguntar por servicios del hotel”
	- “Ver horarios”
	- “Hablar con recepción”
## Lo que deben implementar en la APP
### Pantalla de chat
- Zona de conversación (mensajes del usuario y del chatbot).
- Campo de texto para escribir.
- Botón para enviar mensaje.
- Opcional pero muy recomendable: botones rápidos (chips) con opciones:
	- “Servicios del hotel”
	- “Habitaciones”
	- “Recomendaciones”
	- “Hablar con recepción”
### Lógica del chatbot
1. Reconocer al menos estas intenciones:
	- Preguntas sobre **horarios**.
	- Preguntas sobre **servicios**.
	- Preguntas sobre **habitaciones**.
	- Preguntas sobre **recomendaciones**.
	- Petición de **hablar con recepción**.
2. Devolver una respuesta adecuada según la intención detectada.
3. Tener un mensaje comodín para lo que no entienda (mensaje de error + opciones).
### Extra opcional (si quieres subir el nivel)
Guardar el **historial de mensajes** durante la sesión, por ejemplo en GoogleSheets.
# Desarrollo
![](000%20Assets/P1.%20Creacion%20del%20Chatbot%20del%20Hotel%20Costa%20Azul/P1%20-%20Chatbot%20Hotel%20Costa%20Azul_2.png)
Tras finalizar el proyecto, he hecho con el una plantilla para poder compartirlo. Puedes acceder a ella a traves del siguiente [enlace](https://templates.landbot.io/hotel-costa-azul-5637/).

Enlace para probar Chatbot para el hotel Costa Azul es [Chatbot Hotel](https://landbot.online/v3/H-3311903-K78FFBK92N2L0L4Y/index.html)

El enlace del documento GoogleSheets donde se guardan/consultan las reservas es [reservas hotel](https://docs.google.com/spreadsheets/d/1iqvtJfgEVy3EzKdblNYT8VVvSt3J_mywCCGavzZnO3I/edit?usp=sharing).
