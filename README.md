instrucción de renombrar el archivo .env.example a .env para que funcione correctamente:

---

# Bot de Asistente de IA para WhatsApp (BuilderBot.app)

<p align="center">
  <img src="https://builderbot.vercel.app/assets/thumbnail-vector.png" height="80">
</p>

[![Desplegar en Railway](https://railway.app/button.svg)](https://railway.app/template/6VbbLI?referralCode=jyd_0y)

Este proyecto crea un bot de WhatsApp que se integra con un asistente de IA usando la tecnología de BuilderBot. Permite conversaciones automatizadas y respuestas inteligentes mediante la API de asistente de OpenAI.

## Características

- Flujos de conversación automatizados para WhatsApp
- Integración con la API del asistente de OpenAI
- Independiente del proveedor de WhatsApp
- Respuestas automáticas a preguntas frecuentes
- Recepción y respuesta de mensajes en tiempo real
- Seguimiento de interacciones con clientes
- Funcionalidad expandible a través de activadores (triggers)

## Primeros pasos

1. Clona este repositorio.
2. Instala las dependencias:
   bash
   pnpm install
   
3. Renombra el archivo .env.example a .env y configura las variables de entorno en el archivo .env:
   plaintext
   PORT=3008
   ASSISTANT_ID=tu_assistant_id_de_openai
   OPENAI_API_KEY=tu_openai_api_key
   
4. Ejecuta el servidor de desarrollo:
   bash
   pnpm run dev
   

### Usando Docker (Recomendado)

Este proyecto incluye un Dockerfile para facilitar el despliegue y asegurar entornos consistentes. Para usar Docker:

1. Construye la imagen de Docker:
   bash
   docker build -t whatsapp-ai-assistant .
   
2. Ejecuta el contenedor:
   bash
   docker run -p 3008:3008 --env-file .env whatsapp-ai-assistant
   

Este método asegura que la aplicación funcione en un entorno consistente en diferentes sistemas.

## Uso

El bot está configurado en el archivo src/app.ts. Utiliza la biblioteca BuilderBot para crear flujos y gestionar mensajes. El flujo de bienvenida principal se integra con el asistente de OpenAI para generar respuestas.

## Documentación

Para más información sobre cómo usar y ampliar este bot, consulta la [documentación de BuilderBot](https://builderbot.vercel.app/).

## Contribución

¡Las contribuciones son bienvenidas! No dudes en enviar un Pull Request.

## Licencia

Este proyecto es de código abierto y está disponible bajo la [Licencia MIT](LICENSE).

## Contacto

Para preguntas y soporte, únete a nuestra [comunidad en Discord](https://link.codigoencasa.com/DISCORD) o síguenos en [Twitter](https://twitter.com/leifermendez).

---

Construido con [BuilderBot](https://www.builderbot.app/en) - Potenciando la IA conversacional para WhatsApp.