# Nelson - Discord Ticket & Question Bot

🤖 **Nelson** es un bot de soporte para Discord que facilita la gestión de tickets de ayuda y preguntas, permitiendo a los usuarios comunicarse fácilmente con el staff y mantener todo organizado.

---

## Características

- 🎟️ **Sistema de Tickets**
  - Los usuarios pueden abrir tickets privados para recibir ayuda personalizada.
  - Control de cooldown para evitar abrir múltiples tickets seguidos.
  - Tickets con permisos privados para privacidad.
  - Botón para cerrar tickets con generación automática de transcripciones.
  - Recordatorios automáticos de inactividad.
  - Cierre automático de tickets tras 12 horas sin respuesta.
  - Contador dinámico de tickets abiertos en un canal dedicado.

- ❓ **Sistema de Preguntas**
  - Los usuarios pueden enviar preguntas al staff mediante un formulario modal.
  - Notificación privada al owner y co-owner con opciones para responder o marcar como resuelta.
  - Respuestas enviadas directamente al usuario vía DM.
  - Registro y log de preguntas y respuestas para auditoría.

- 🔐 **Control de permisos**
  - Solo el owner y co-owner pueden gestionar tickets y responder preguntas.
  - Protección y privacidad mediante permisos ajustados en los canales.

- 📁 **Registros**
  - Transcripciones guardadas localmente.
  - Logs de tickets cerrados y preguntas respondidas.

---

## Requisitos

- Python 3.8 o superior
- Librerías:
  - `discord.py` (versión compatible con UI/Buttons/Modals)
  - `python-dotenv`

---

## Instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/tu_usuario/nelson-bot.git
   cd nelson-bot

2. Instala las dependencias:

pip install -r requirements.txt


3. Crea un archivo .env con las siguientes variables:

DISCORD_TOKEN=tu_token_aqui
OWNER_ID=id_owner
CO_OWNER_ID=id_co_owner
STAFF_ROLE_ID=id_rol_staff
GUILD_ID=id_de_tu_servidor


4. Ejecuta el bot:

python bot.py




---

Uso

Ejecuta /setup en el canal donde quieres desplegar el panel de soporte (solo para owner o co-owner).

Usuarios podrán abrir tickets o hacer preguntas desde el panel.

El staff gestionará tickets y responderá preguntas desde DMs.

Los tickets inactivos reciben recordatorios y se cierran automáticamente si no hay actividad.



---

Archivos y Logs

Transcripciones de tickets en: logs/transcripts/

Preguntas registradas en: logs/questions.txt

Respuestas a preguntas en: logs/question_responses.txt

Historial de tickets cerrados en: logs/closed_tickets.txt

Registro de cierres automáticos en: logs/ticket_history.txt



---

Contribuciones

¡Contribuciones bienvenidas! Si quieres agregar nuevas funciones o corregir errores, abre un pull request.


---

Licencia

MIT License © 2025 Tu Nombre


---

Nelson - Un bot sencillo pero potente para manejar soporte en Discord.
