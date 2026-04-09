# ⚡ ElectroTech API

API RESTful escalable desarrollada en equipo para gestionar productos, usuarios y recursos de una tienda de electrónica. Incluye panel de administración con vistas dinámicas, autenticación segura y control de accesos por roles.

🎥 **[Ver video de demostración (3 min)](https://youtu.be/MvIxc-i6oFM)**

---

## 🚀 Tecnologías utilizadas

| Área | Tecnologías |
|---|---|
| Backend | Node.js, Express.js |
| Base de datos | MySQL |
| Vistas (admin) | EJS |
| Seguridad | bcrypt, dotenv |
| Frontend | HTML, CSS, JavaScript |
| Control de versiones | Git (ramas por feature) |

---

## 🏗️ Arquitectura

El proyecto sigue el patrón **MVC (Modelo - Vista - Controlador)** para mantener el código modular, organizado y fácil de escalar.

```
electrotech-api/
├── Tp_integrador_BACK/
│   ├── controllers/     # Lógica de negocio
│   ├── models/          # Modelos de datos y consultas SQL
│   ├── routes/          # Definición de endpoints
│   ├── views/           # Vistas dinámicas con EJS (panel admin)
│   └── middlewares/     # Autenticación y autorización
├── Tp_integrador_FRONT/ # Interfaz del cliente
├── tp_progra_3.sql      # Script de base de datos
└── .env.example         # Variables de entorno de ejemplo
```

---

## ✨ Funcionalidades principales

- **CRUD completo** de productos (crear, ver, editar, eliminar)
- **Autenticación** con contraseñas hasheadas usando bcrypt
- **Control de accesos por roles** — administrador y usuario con permisos diferenciados
- **Panel de administración** con vistas dinámicas renderizadas con EJS
- **API RESTful** con endpoints organizados y respuestas en JSON
- **Variables de entorno** gestionadas con dotenv para mayor seguridad

---

## ⚙️ Instalación y uso

### Requisitos previos
- Node.js v18+
- MySQL

### Pasos

```bash
# 1. Clonar el repositorio
git clone https://github.com/Portu004/electrotech-api.git
cd electrotech-api

# 2. Instalar dependencias
npm install

# 3. Configurar variables de entorno
cp .env.example .env
# Completar los valores en el archivo .env

# 4. Importar la base de datos
mysql -u root -p < tp_progra_3.sql

# 5. Iniciar el servidor
npm start
```

El servidor corre por defecto en `http://localhost:3000`

---

## 🔐 Variables de entorno

Crear un archivo `.env` en la raíz con las siguientes variables:

```env
DB_HOST=localhost
DB_USER=tu_usuario
DB_PASSWORD=tu_contraseña
DB_NAME=electrotech
PORT=3000
JWT_SECRET=tu_secreto
```

---

## 👥 Equipo de desarrollo

Proyecto desarrollado en equipo de 3 personas utilizando **Git Flow** con ramas por feature y revisión de código colaborativa.

| Desarrollador | GitHub |
|---|---|
| Matias Goncalves | [@Portu004](https://github.com/Portu004) |
| Nicolas Macri | [@nmacri9](https://github.com/nmacri9) |
| Mateo Nicolas Garcia | [@Mateogarcia666](https://github.com/Mateogarcia666) |

---

## 📄 Licencia

Este proyecto está bajo la licencia [MIT](LICENSE).
