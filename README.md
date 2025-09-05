## 🧑‍💻 User CRUD App
Esta aplicación fue desarrollada como parte de un proyecto de aprendizaje con el objetivo de construir una app en React utilizando Vite.js, que permite Crear, Leer, Actualizar y Eliminar (CRUD) usuarios mediante una API local simulada con JSON Server. Se enfoca en el manejo eficiente de formularios, validaciones dinámicas, componentes reutilizables y una experiencia visual clara y responsiva.

Se integran múltiples hooks personalizados, validaciones con Zod, formularios reactivos con `react-hook-form`, y modales reutilizables mediante la propiedad `children`, todo dentro de una arquitectura modular y escalable.

## 🚀Demo en línea  
**🔗Disponible solo en servidor local**

## 🎯 Objetivo del proyecto

Construir una aplicación web funcional e interactiva en React usando Vite.js, que permita al usuario:

- Crear nuevos usuarios mediante un formulario validado.
- Visualizar todos los usuarios en tarjetas personalizadas.
- Editar usuarios existentes con formularios dinámicos.
- Eliminar usuarios con confirmación visual.
- Validar entradas con mensajes claros y estructura semántica.

Este proyecto refuerza habilidades clave como:

- Manejo de formularios reactivos con `react-hook-form`.
- Validaciones con `zod` y `@hookform/resolvers`.
- Consumo de APIs RESTful con `axios`.
- Manejo de estados, efectos y renderizado condicional.
- Creación de hooks personalizados para encapsular lógica de peticiones.
-  Uso de `children` para componentes reutilizables como modales y botones.
- Diseño modular, responsivo y accesible. 

## ⚛️Tecnologías usadas⚡

### Tecnologías principales

| Herramienta / Lenguaje | Uso principal |
|------------------------|---------------|
| **React**              | Construcción modular de componentes. |
| **Vite.js**            | Entorno rápido de desarrollo y bundling. |
| **JavaScript (ES6+)**  | Lógica de búsqueda, validaciones y renderizado. |
| **CSS / SCSS**         | Estilos personalizados y estructurados. |
| **HTML / JSX**         | Estructura declarativa de la app. |
| **Axios**              | Comunicación con la API. |
| **React Icons**        | Íconos personalizables y semánticos. |
| **React Hook Form**    | Manejo eficiente de formularios. |
| **Zod**                | Validaciones declarativas y robustas. |
| **ESLint + Plugins**   | Liting para calidad y consistencia del código. |

### APIs y funcionalidades externas

| Tecnología / API              | Funcionalidad |
|-------------------------------|---------------------------|
| **JSON Server**               | Simulación de API RESTful para usuarios. |
| **Custom Hook(useUsersCrud)** | Encapsula lógica de peticiones HTTP. |
| **Custom Hook(usePagination)**| Encapsula lógica para la paginación en los usuarios. |
| **Custom Hook(useModal)**     | Encapsula lógica para el funcionamiento del modal. |

### Lógica y estructura con React

- **`useState`**: Control de inputs, errores, modales y usuarios.
- **`useEffect`**: Carga inicial de usuarios y sincronización de estados.
- **`react-hook-form`**: Captura y validación de datos del formulario.
- **`zod`**: Validaciones declarativas y reutilizables.
- **`useUsersCrud`**: Custom hook para manejar todas las peticiones HTTP (GET, POST, PUT, PATCH, DELETE).
- **Propiedad `children`**: Para modales, botones y componentes reutilizables.
- **Componentes personalizados.**: `UserCard`, `Form`, `Modal`, `LoadingScreen`, `Pagination`, `UserContent`.

### Experiencia del usuario

- Loader con un carrusel animado que contiene tarjetas de usuario creadas al azar(sin mostrar datos).
- Carga de los datos en tarjetas de usuarios, cada usuario contiene sus respectivos datos preestablecidos en el archivo json.
- Paginación en botones que muestra seis usuarios por página.
- Formulario dinámico que cambia entre modo creación y edición.
- Validaciones claras con mensajes personalizados.
- Modales de confirmación tras crear, editar o eliminar.
- Diseño responsivo para escritorio y móvil.
- Interacción fluida y retroalimentación visual inmediata.

## 🗂️Estructura del proyecto

```bash
📁 S04E04/
|   ├── 📁 node_modules/
|   ├── 📁 public/
|   ├── 📁 src/
│   |    └── 📁 assets/
│   |    └── 📁 components/
│   |    |   └── Form.jsx
|   |    |   └── LoadingScreen.jsx
|   |    |   └── Modal.jsx
|   |    |   └── Pagination.jsx
|   |    |   └── UserCard.jsx
|   |    |   └── UserContent.jsx
│   |    └── 📁 hooks/
|   |    |   └── useCrud.jsx
|   |    |   └── useModal.jsx
|   |    |   └── usePagination.jsx
│   |    └── 📁 lib/
│   |    |   └── utils.js
│   |    └── 📁 styles/
│   |    |   └── App.css
|   |    |   └── Form.css
|   |    |   └── LoadingScreen.css
|   |    |   └── Modal.scss
|   |    |   └── Pagination.css
|   |    |   └── UserCard.css
|   |    |   └── UserContent.css
|   |    └── App.jsx
|   |    └── index.css
|   |    └── main.jsx
|   └── db.json
```

## 🧠Funcionalidades principales

- Listado de usuarios con tarjetas personalizadas.
- Formulario para crear y editar usuarios:

    **`email`**
    **`password`**
    **`first_name`**
    **`last_name`**
    **`birthday`**
    **`image_url`**(opcional)

- Validaciones con `zod` y `react-hook-form`.
- Modales de confirmación tras acciones exitosas.
- Hooks personalizados para peticiones HTTP.  
- Diseño modular y componentes reutilizables.
- Estilos SCSS por componente.
- Propiedad `children` para modales y botones.
- Experiencia responsiva y accesible.

## 🛠️Instalación local

1. Clona este repositorio:

```bash
git clone https://github.com/Clic-stack/UserCrud-with-Local-Server.git
```

2. Instala las dependencias:

```bash
npm install
```

3. Inicia el servidor local (JSON Server):

```bash
npm run api
```

4. Ejecuta el proyecto:

```bash
npm run dev
```

## 🎨Autor  
Desarrollado por Clio Salgado como parte del módulo de React en Academlo, con el objetivo de consolidar habilidades en desarrollo frontend, validaciones, consumo de APIs y diseño modular.

---

🔽 **English version below** 🔽

## 🧑‍💻 User CRUD App
This application was developed as part of a learning project with the goal of building a React app using Vite.js that enables Create, Read, Update, and Delete (CRUD) operations for users through a locally simulated API using JSON Server. It focuses on efficient form handling, dynamic validations, reusable components, and a clear, responsive visual experience.

It integrates multiple custom hooks, validations with Zod, reactive forms via `react-hook-form`, and reusable modals using the `children` property—all within a modular and scalable architecture.

## 🚀Demo en línea  
**🔗Available only on local server**

## 🎯 Project Objective

Build a functional and interactive web application in React using Vite.js, allowing users to:

- Create new users through a validated form.
- Display all users in personalized cards.
- Edit existing users with dynamic forms.
- Delete users with visual confirmation.
- Validate inputs with clear messages and semantic structure.

This project strengthens key skills such as:

- Reactive form handling with `react-hook-form`.
- Validations using `zod` and `@hookform/resolvers`.
- RESTful API consumption with `axios`.
- State and effect management with conditional rendering.
- Custom hooks to encapsulate API logic.
- Use of `children` for reusable components like modals and buttons.
- Modular, responsive, and accessible design. 

## ⚛️Technologies Used⚡

### Core Technologies

| Tool / Language        | Primary Use |
|------------------------|---------------|
| **React**              | Modular component construction. |
| **Vite.js**            | Fast development environment and bundling. |
| **JavaScript (ES6+)**  | Logic for search, validations, and rendering. |
| **CSS / SCSS**         | Structured and customized styling. |
| **HTML / JSX**         | Declarative app structure. |
| **Axios**              | API communication. |
| **React Icons**        | Semantic and customizable icons. |
| **React Hook Form**    | Efficient form management. |
| **Zod**                | Declarative and robust validations. |
| **ESLint + Plugins**   | Code quality and consistency. |

### External APIs and Features

| Technology / API              | Functionality |
|-------------------------------|---------------------------|
| **JSON Server**               | Simulated RESTful API for users. |
| **Custom Hook(useUsersCrud)** | Encapsulates HTTP request logic. |
| **Custom Hook(usePagination)**| Handles pagination logic for users. |
| **Custom Hook(useModal)**     | Manages modal functionality. |

### React Logic and Structure

- **`useState`**: Controls inputs, errors, modals, and user data.
- **`useEffect`**: Loads initial users and syncs state.
- **`react-hook-form`**: Captures and validates form data.
- **`zod`**: Reusable and declarative validations.
- **`useUsersCrud`**: Custom hook for all HTTP requests (GET, POST, PUT, PATCH, DELETE).
- **`children` property**: For reusable modals, buttons, and components.
- **Custom Components**: `UserCard`, `Form`, `Modal`, `LoadingScreen`, `Pagination`, `UserContent`.

### User Experience

- Loader with an animated carousel displaying randomly styled user cards (without actual data).
- User data loaded into cards, each showing predefined JSON data.
- Pagination buttons displaying six users per page.
- Dynamic form switching between create and edit modes.
- Clear validations with personalized messages.
- Confirmation modals after create, edit, or delete actions.
- Responsive design for desktop and mobile.
- Smooth interaction and immediate visual feedback.

## 🗂️Project Structure

```bash
📁 S04E04/
|   ├── 📁 node_modules/
|   ├── 📁 public/
|   ├── 📁 src/
│   |    └── 📁 assets/
│   |    └── 📁 components/
│   |    |   └── Form.jsx
|   |    |   └── LoadingScreen.jsx
|   |    |   └── Modal.jsx
|   |    |   └── Pagination.jsx
|   |    |   └── UserCard.jsx
|   |    |   └── UserContent.jsx
│   |    └── 📁 hooks/
|   |    |   └── useCrud.jsx
|   |    |   └── useModal.jsx
|   |    |   └── usePagination.jsx
│   |    └── 📁 lib/
│   |    |   └── utils.js
│   |    └── 📁 styles/
│   |    |   └── App.css
|   |    |   └── Form.css
|   |    |   └── LoadingScreen.css
|   |    |   └── Modal.scss
|   |    |   └── Pagination.css
|   |    |   └── UserCard.css
|   |    |   └── UserContent.css
|   |    └── App.jsx
|   |    └── index.css
|   |    └── main.jsx
|   └── db.json
```

## 🧠Key Features

- User listing with personalized cards.
- Form for creating and editing users:

    **`email`**
    **`password`**
    **`first_name`**
    **`last_name`**
    **`birthday`**
    **`image_url`**(optional)

- Validations with `zod` and `react-hook-form`.
- Confirmation modals after successful actions.
- Custom hooks for API requests.  
- Modular design and reusable components.
- SCSS styling per component.
- Use of `children` for modals and buttons.
- Responsive and accessible user experience.

## 🛠️Local Installation

1. Clone this repository:

```bash
git clone https://github.com/Clic-stack/UserCrud-with-Local-Server.git
```

2. Install dependencies:

```bash
npm install
```

3. Start the local server (JSON Server):

```bash
npm run api
```

4. Run the project:

```bash
npm run dev
```

## 🎨Author
Developed by Clio Salgado as part of the React module at Academlo, with the goal of strengthening frontend development skills, validations, API consumption, and modular design.
