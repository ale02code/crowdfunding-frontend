# **Plataforma de Crowdfunding** 💰💹

## **Descripción General** 🗒

La **Plataforma de Crowdfunding** es un sistema web diseñado para conectar a personas o grupos que buscan recaudar fondos con potenciales donantes interesados en apoyar causas, proyectos innovadores, o productos creativos.

Los creadores de campañas pueden establecer metas económicas, descripciones detalladas y recompensas para incentivar las donaciones. La plataforma se encarga de gestionar cada etapa del proceso: desde la creación y promoción de campañas hasta el manejo de transacciones seguras y la administración de usuarios.

---

## **Requisitos del Frontend** 🌐

El **Frontend** proporciona la interfaz que los usuarios emplean para interactuar con las funcionalidades de la plataforma. Debe ser visualmente atractivo, responsivo y fácil de usar.

### **1. Páginas principales**

- **Inicio**:
  - Mostrar campañas destacadas, nuevas o populares.
  - Proveer filtros por categorías y una barra de búsqueda dinámica.
- **Detalles de la campaña**:
  - Información detallada como título, descripción, barra de progreso, monto objetivo, recompensas y opciones para donar.
- **Página de perfil**:
  - Visualizar campañas creadas por el usuario, historial de donaciones y estadísticas generales.

### **2. Formularios interactivos**

- **Creación de campañas**:
  - Permitir a los usuarios ingresar título, descripción, monto objetivo, fecha límite, y subir imágenes.
  - Validaciones en tiempo real para cada campo.
- **Registro/Login**:
  - Crear formularios con validaciones de correo, contraseñas seguras y mensajes de error específicos.
- **Donaciones**:
  - Seleccionar el monto de donación y método de pago (Stripe o PayPal).

### **3. Navegación fluida**

- Implementar navegación entre páginas con **React Router**.
- Crear un sistema de rutas privadas para restringir el acceso a ciertas páginas (como la gestión de campañas).

### **4. Gestión del estado**

- Usar **Context API** o **Redux** para manejar:
  - Campañas disponibles y detalles de usuario.
  - Historial de donaciones y mensajes de notificación.
- Integrar notificaciones dinámicas (como confirmación de donación exitosa).

### **5. Diseño y Componentización**

- Crear componentes reutilizables como:
  - Tarjetas para campañas.
  - Barras de progreso para recaudaciones.
  - Formularios dinámicos.
- Usar librerías como **Tailwind CSS** o **Bootstrap** para estilizar de manera eficiente y garantizar la responsividad.

### **6. Conexión con el Backend**

Consumir las APIs necesarias para:

- **Obtener datos**:
  - Campañas disponibles.
  - Historial de interacciones de los usuarios.
- **Enviar información**:
  - Datos de creación de campañas.
  - Registro de donaciones.

### **7. Pruebas**

- Validar la funcionalidad del Frontend con herramientas como **Jest** o **Cypress** para:
  - Formularios de validación.
  - Navegación entre rutas.
  - Confirmación de pagos y eventos.

---

## **Requisitos del Backend** 🛠️

El **Backend** maneja la lógica del negocio, la administración de datos, la seguridad y la integración con servicios externos.

### **1. Estructura y Administración de Datos**

- Diseñar un modelo de datos relacional utilizando **PostgreSQL**:
  - Usuarios (nombre, correo, contraseña cifrada).
  - Campañas (título, descripción, monto objetivo, progreso, creador).
  - Donaciones (usuario, campaña, monto, método de pago).

### **2. API RESTful**

- Crear endpoints organizados para:
  - **Campañas**:
    - Listar todas las campañas activas.
    - Crear, editar y eliminar campañas (solo por sus propietarios).
  - **Donaciones**:
    - Registrar una nueva donación.
    - Obtener el historial de donaciones de un usuario.
  - **Usuarios**:
    - Registro y autenticación.
    - Perfil con campañas y donaciones relacionadas.

### **3. Seguridad**

- Implementar autenticación con **JWT (JSON Web Tokens)** para manejar sesiones de usuarios.
- Proteger los datos sensibles con cifrado (por ejemplo, contraseñas usando **bcrypt**).
- Validar todas las entradas para evitar vulnerabilidades como **SQL Injection** o **Cross-Site Scripting (XSS)**.

### **4. Integración de Pagos**

- Integrar pasarelas de pago seguras como **Stripe** o **PayPal**:
  - Configurar transacciones seguras.
  - Notificar al sistema en tiempo real sobre pagos completados o rechazados.

### **5. Pruebas**

- Probar la API usando herramientas como **Postman** o **Insomnia**.
- Crear pruebas unitarias con **Pytest** para validar la lógica de negocio y asegurar la integridad de los datos.

---

## **Tecnologías Utilizadas** 💻

### **Frontend**

- **React** (framework principal).
- **Vite** (entorno de desarrollo rápido).
- **Tailwind CSS** o **Bootstrap** (estilización).
- **React Router** (navegación).

### **Backend**

- **Django** o **Flask** (framework web).
- **PostgreSQL** (base de datos relacional).
- **Stripe/PayPal SDK** (integración de pagos).

---

## **Contacto** 📫

¿Tienes preguntas o sugerencias sobre este proyecto? ¡Contáctame!

### Frontend Developer

- **GitHub**: [ale02code](https://github.com/ale02code)
- **Correo Electrónico**: [chchacon02@gmail.com](mailto:chchacon02@gmail.com)

### Backend Developer

- **GitHub**: [diegosowtf](https://github.com/diegosowtf)
- **Correo Electrónico**: [diegosandoval.ismael@gmail.com](mailto:diegosandoval.ismael@gmail.com)
