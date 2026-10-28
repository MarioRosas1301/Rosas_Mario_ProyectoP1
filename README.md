# 🏔️ Proyecto P1 - Sitio Web Turístico: Descubre Ecuador

¡Bienvenido al repositorio oficial del **Proyecto P1** para la asignatura de **Programación Web**! Este portal web promociona los principales destinos turísticos de las regiones de Ecuador, cumpliendo rigurosamente con los estándares web modernos, maquetación adaptativa y empaquetado mediante contenedores Docker.

---

## 👨‍💻 Información del Estudiante
* **Autor:** Mario Rosas
* **Asignatura:** Programación Web
* **Carrera:** Ingeniería / Software
* **Proyecto:** Primer Parcial - Sitio Web Turístico
* **Modalidad:** Individual
* **Repositorio GitHub:** [MarioRosas1301/Rosas_Mario_P1](https://github.com/MarioRosas1301/Rosas_Mario_ProyectoP1)
* **Docker Hub:** [`mirosas/proyecto-p1:v1`](https://hub.docker.com/r/mirosas/proyecto-p1)

---

## 📋 Descripción del Proyecto

El proyecto consiste en el diseño y desarrollo de una plataforma web atractiva, accesible y totalmente responsiva dedicada a la promoción turística de Cuenca, Ecuador. La plataforma organiza la oferta turística en secciones claras que facilitan al usuario la consulta de destinos, galerías fotográficas, paquetes de viaje con costos y servicios, itinerarios detallados y un formulario de contacto validado.

---

## ✨ Requerimientos y Contenido del Sitio

El sitio web está estructurado en las siguientes secciones principales:

1. **🏠 Inicio:** Presentación visual impactante del sitio, identidad de marca, hero banner promocional y menú de navegación global.
2. **📍 Destinos Turísticos:** Exhibición de 4 destinos emblemáticos con fotografías y descripciones detalladas:
   * *Centro Histórico* 
   * *Parque Nacional Cajas* 
   * *Ingapirca ancestral* 
   * *Gualaceo & Chordeleg* 
3. **🖼️ Galería:** Mosaico fotográfico organizado y optimizado de los paisajes y lugares turísticos.
4. **📦 Paquetes Turísticos:** Mínimo 3 opciones comerciales detalladas con precio, duración y servicios incluidos:
   * *Pack Esencia cuencana* ($89 / 1D)
   * *Pack Entre ciudad y Andes* ($189 / 3D-2N)
   * *Pack Cuenca sin prisa ($329 / 5D-4N)
5. **📅 Itinerarios:** Cronograma de actividades turísticas organizadas por días y horarios.
6. **📩 Formulario de Consultas:** Sección interactiva con validaciones nativas de HTML5 (campos obligatorios, formato de email, selección de destino) para solicitudes de información.

---

## 🛠️ Requisitos Técnicos e Implementación

* **HTML5 Semántico:** Estructura limpia y accesible utilizando etiquetas estructurales (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`).
* **CSS3 Moderno:** Hojas de estilo externas y limpias.
* **Diseño Responsivo (Mobile First):** Maquetación fluida y adaptable a dispositivos móviles, tablets y monitores mediante **Flexbox** y **CSS Grid**.
* **Navegación Orgánica:** Menú claro, accesible y estéticamente alineado con la temática turística.

---

## 🐳 Ejecución y Despliegue con Docker

El proyecto se encuentra empaquetado dentro de una imagen liviana alimentada por **Nginx sobre Alpine Linux**. Puedes desplegar el sitio localmente mediante cualquiera de los siguientes dos métodos:

### Opción A: Descargando la imagen oficial desde Docker Hub (Recomendado)

Ejecuta directamente la imagen publicada en Docker Hub en el puerto `8080`:

```bash
docker run -d -p 8080:80 --name app-turismo-hub mirosas/proyecto-p1:v1
```

### Opción B: Compilando la imagen localmente desde el código fuente

1. Clona el repositorio e ingresa a la carpeta del proyecto:
   ```bash
   git clone https://github.com/MarioRosas1301/Rosas_Mario_P1.git
   cd Rosas_Mario_P1
   ```

2. Construye la imagen Docker localmente:
   ```bash
   docker build -t proyecto-p1:v1 .
   ```

3. Ejecuta el contenedor:
   ```bash
   docker run -d -p 8080:80 --name app-turismo-local proyecto-p1:v1
   ```

---

## 🌐 Visualización en el Navegador

Una vez iniciado el contenedor de Docker por cualquiera de las dos opciones, abre tu navegador web e ingresa a la siguiente dirección:

👉 **`http://localhost:8080`**

---

## 📁 Estructura del Repositorio

```text
Rosas_Mario_P1/
├── index.html              # Página principal y estructura del sitio
├── css/
│   └── styles.css          # Estilos globales, Flexbox/Grid y Media Queries
├── assets/
│   ├── img/                # Imágenes de destinos, galería y paquetes
│   └── icons/              # Iconografía del sitio
├── Dockerfile              # Configuración del contenedor Nginx Alpine
├── presentacion_proyecto_p1.html  # Diapositivas interactivas de exposición
└── README.md               # Documentación general del proyecto
```