# 🧮 Matemágica – Simulador de costos para clases de apoyo

**Matemágica** es una herramienta web interactiva que permite a los estudiantes de nivel secundario **calcular el costo de una clase particular de matemática** en función de la cantidad de personas, horas, modalidad y curso. Además, incluye un formulario de contacto para solicitar más información o reservar una clase.

Este proyecto fue desarrollado como **entrega final de un curso de JavaScript**, aplicando conceptos como manipulación del DOM, funciones asíncronas, promesas, uso de librerías externas (SweetAlert2) y validación de formularios.

---

## 📌 Descripción

La página permite al usuario:

- Ingresar sus datos personales (nombre, teléfono).
- Seleccionar el **curso** (ej: 1° año, 2° año, etc.).
- Elegir la **modalidad** de clase (presencial, virtual, etc.).
- Indicar la **cantidad de personas** y **horas** de clase.
- **Agregar temas a estudiar** desde una lista dinámica.
- **Calcular automáticamente el costo total** de la clase.
- Enviar el formulario de contacto.

Todo esto se realiza con una interfaz amigable y validaciones, mostrando mensajes de éxito o error usando **SweetAlert2**.

---

## 🚀 Tecnologías utilizadas

| Tecnología                | Uso                                                      |
|---------------------------|----------------------------------------------------------|
| HTML5                     | Estructura semántica del sitio                          |
| CSS3 (archivo `estilo.css`) | Diseño responsivo y estilos personalizados           |
| JavaScript (ES6+)         | Lógica de negocio, manipulación del DOM, eventos        |
| SweetAlert2               | Notificaciones y alertas modernas y atractivas          |
| Promesas / async-await    | Manejo de operaciones asíncronas (ej. carga de datos)   |
| Google Fonts              | Fuente **Raleway** para una tipografía moderna          |

---

## 📂 Estructura del proyecto (esperada)
```bash
Matemágica/
│
├── index.html # Página principal
├── Eventos.PNG # Capturas de pantalla (documentación)
├── Eventos2.PNG
├── Eventos3.PNG
│
├── css/
│ ├── estilo.css # CSS compilado desde SCSS
│ └── estilo.css.map # Sourcemap del CSS
│
├── scss/
│ └── style.scss # Archivo fuente SASS/SCSS
│
├── javascript/
│ ├── main.js # Lógica principal (cálculo, eventos, fetch)
│ └── validaciones.js # Validaciones del formulario y helpers
│
├── data/
│ ├── curso.json # Lista de cursos disponibles
│ ├── modalidad.json # Modalidades (presencial, virtual, etc.)
│ └── temas.json # Temas de estudio para agregar
│
├── imagenes/
│ └── calculador.png 
│
└── README.md # Este archivo
```
## 🔧 Instalación y uso local

1. **Clona o descarga** este repositorio en tu computadora.
2. Asegúrate de mantener la estructura de carpetas indicada.
3. Abre el archivo `index.html` en tu navegador web.
4. Para una mejor experiencia, utiliza un servidor local (por ejemplo, Live Server de VS Code).

No requiere instalación de dependencias adicionales (las librerías se cargan vía CDN).

---

## 📝 Funcionalidades principales

### ✅ Selectores dinámicos
- Cursos y modalidades se cargan mediante JavaScript (pueden venir de un array o de una API simulada).
- Temas disponibles se muestran en un `<select>` y el usuario puede agregarlos a una lista personalizada.

### ✅ Cálculo de costo
- Precio base: $8000 por persona por hora para 1 alumno.  
- $7000 por persona por hora para grupos de 2 o más.
- El total se actualiza automáticamente cuando cambian las cantidades.

### ✅ Validación y envío
- El formulario valida que todos los campos estén completos.
- Al enviar, se muestra un mensaje de éxito (SweetAlert) con el resumen de la consulta.

### ✅ Interfaz responsive
- Diseño adaptado a dispositivos móviles y escritorio.

---

## 🤔 ¿Cómo contribuir?

Si deseas mejorar el proyecto:
1. Realiza un fork del repositorio.
2. Crea una rama con tu feature (`git checkout -b mejora-calculo`).
3. Haz commit de tus cambios.
4. Abre un Pull Request.

También puedes reportar errores o sugerir ideas a través de los issues del proyecto (si está alojado en GitHub).

---

## 📄 Licencia

Este proyecto fue creado con fines educativos como parte de un curso de JavaScript. Puede ser utilizado libremente para aprendizaje.

---

**Desarrollado por Melina Noelia Andrada** – Entrega final del curso de JavaScript.  
¡Aprobá tus exámenes con Matemágica! 🧙‍♂️✨
