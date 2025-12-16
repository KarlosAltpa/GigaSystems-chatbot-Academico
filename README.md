# GigaSystems-chatbot-Academico
Desarrollamos un Chatbot Académico Inteligente capaz de atender solicitudes estudiantiles de manera automática, especialmente la gestión y emisión de certificados, proporcionando respuestas precisas, validaciones automáticas y orientaciones claras según la normativa universitaria.

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/21cb70a5-7db6-4fb5-8935-439ee94e3abb" />

# 🌐 Proyecto Web UTEG – Plataforma Informativa con Chat Estudiantil

## 📌 Descripción del Proyecto

Este proyecto consiste en el desarrollo de una **aplicación web moderna** para la **Universidad Tecnológica Empresarial del Ecuador (UTEG)**, creada con el objetivo de **informar, interactuar y brindar asistencia a los estudiantes** mediante un sitio web responsivo y un chat estudiantil automatizado.

La aplicación fue desarrollada utilizando el **IDE Orquídeas**, aprovechando sus créditos gratuitos, y está lista para su despliegue.

---

## 🎯 Objetivo

Desarrollar un sitio web:

* Moderno y responsivo
* Accesible y optimizado
* Con sistema de autenticación de estudiantes
* Con un **chat informativo integrado mediante n8n**

---

## 🛠️ Tecnologías Utilizadas

* **React** (SPA con React Router)
* **TypeScript**
* **Tailwind CSS**
* **Supabase Auth** (registro e inicio de sesión)
* **n8n** (webhook para chat estudiantil)
* **Orquídeas IDE**

---

## 🎨 Diseño y Branding

* Uso del **logo oficial de UTEG**
* Imágenes representativas de las **carreras universitarias**
* Paleta de colores institucional basada en:

  * Azul corporativo
  * Gris
  * Color de acento
* Tipografía moderna y legible
* Variables CSS personalizadas para facilitar el mantenimiento del diseño

---

## 🧱 Arquitectura de la Aplicación

La aplicación sigue una arquitectura **SPA (Single Page Application)** con una estructura clara y modular:

```
src/
├── componentes/    # Componentes reutilizables
├── páginas/        # Vistas principales
├── servicios/      # Integración con APIs
├── lib/            # Utilidades y sesión
├── estilos/        # Configuración de estilos
├── activos/        # Imágenes y recursos
├── App.tsx         # Componente principal
└── index.tsx       # Punto de entrada
```

---

## 🧭 Navegación Principal

* **Inicio (/)**: Información general de UTEG y sus carreras
* **Servicios (/services)**: Servicios educativos de grado y posgrado
* **Login (/login)**: Registro e inicio de sesión
* **Estudiante (/estudiante)**: Área protegida con acceso al chat
* **Chat (/chat)**: Chat informativo conectado a n8n
* **404**: Página para rutas no encontradas

---

## 🔐 Autenticación y Seguridad

* Registro e inicio de sesión con validaciones robustas
* Se aceptan correos que terminen en **@gmail.com**
* Gestión de usuarios mediante **Supabase**
* Rutas protegidas para usuarios autenticados
* Uso de **variables de entorno** para la URL del webhook
* No se exponen credenciales sensibles

---

## 🤖 Chat Estudiantil

* Acceso solo para usuarios autenticados
* Integración con **n8n mediante Webhook**
* Envío de mensajes con `{ mensaje, id }`
* Respuestas renderizadas como **Markdown seguro**
* Historial de conversación
* Manejo de errores y control de estados de carga

---

## ⚙️ Configuración del Proyecto

### Variable de Entorno

Crear un archivo `.env` con la siguiente variable:

```
REACT_APP_API_BASE_URL=https://gigasystems6.app.n8n.cloud/webhook/Estudiantes
```

---

## ▶️ Ejecución Local

```bash
npm install
npm start
```

---

## ♿ Accesibilidad y Rendimiento

* Componentes accesibles con roles ARIA
* Buen contraste de colores (WCAG AA)
* Navegación por teclado
* Optimización de imágenes y carga diferida
* Código limpio y comentado

---

## 📌 Estado del Proyecto

✔ Funcional
✔ Listo para despliegue
✔ Documentado
✔ Cumple con los criterios académicos solicitados

---

## 👨‍🎓 Autor

Proyecto desarrollado por Grupo 2 GygaSistems como parte de un trabajo académico para la **Universidad Tecnológica Empresarial del Ecuador (UTEG)**.

A continuacion les comparto el Link de la paguina:

https://uteg-web-app-development-1.vercel.app/

MUCHAS GRACIAS POR SU ATENCION.
