# TaskFlow

TaskFlow es una aplicación web para organizar tus tareas del día a día. Puedes agregar tareas, asignarles una categoría y un nivel de importancia, marcarlas como completadas cuando termines, y eliminarlas cuando ya no las necesites. Todo desde una interfaz sencilla en el navegador.

---

## ¿Cómo está organizado el proyecto?

```
TaskFlow/
├── public/
│   ├── CSS/
│   │   └── styles.css        # Apariencia visual de la app
│   └── js/
│       └── app.js            # Lo que hace la app en el navegador
├── index.html                # La página principal
├── server.js                 # El servidor que corre detrás de todo
├── package.json
└── package-lock.json
```

---

## ¿Con qué está hecho?

| Parte | Herramienta |
|-------|-------------|
| Servidor | Node.js + Express 5 |
| Página web | HTML5, CSS3, JavaScript |
| Comunicación | API REST (JSON) |
| Guardado de datos | En memoria (se reinician al cerrar el servidor) |
| Desarrollo | Nodemon |

---

## ¿Cómo lo corro?

### 1. Clona el repositorio

```bash
git clone https://github.com/Alexis4rias/TaskFlow.git
cd TaskFlow
```

### 2. Instala lo necesario

```bash
npm install
```

### 3. Enciende el servidor

Si estás trabajando en el proyecto y quieres que se actualice solo al guardar cambios:
```bash
npm run dev
```

Si solo quieres correrlo normalmente:
```bash
npm start
```

### 4. Ábrelo en el navegador

```
http://localhost:3000
```

> ⚠️ **Importante:** No abras el archivo `index.html` directo ni uses el botón "Go Live" de VS Code. La app necesita correr desde el servidor para funcionar bien. Si no, las tareas no cargan.

## ¿Qué puedes hacer con la app?

- ✅ Agregar tareas con título, descripción, categoría y prioridad
- ✅ Marcar una tarea como terminada (o regresarla a pendiente)
- ✅ Borrar tareas que ya no necesitas
- ✅ Filtrar las tareas por categoría
- ✅ Ver cuántas tareas tienes en total y cuántas ya completaste
- ✅ La app valida que el título no esté vacío antes de guardar

---

## Cosas a tener en cuenta

- Las tareas **no se guardan** si apagas el servidor. Cada vez que lo vuelves a encender, regresa a los datos de ejemplo. Aún no hay base de datos.
- El servidor se encarga tanto de mostrar la página web como de guardar y entregar las tareas. Todo desde el mismo lugar.

---

## Autor

**Alexis Arias**  
Estudiante de Ingeniería en Sistemas Computacionales  
Universidad de Montemorelos · Generación 2025–2026