# Festival DevOps 2026

## Descripción

Este proyecto tiene como objetivo aplicar conceptos fundamentales de Git, GitHub, Docker y Docker Compose mediante el desarrollo de una aplicación sencilla para la gestión y promoción de un festival.

Durante el desarrollo se utilizaron ramas para separar funcionalidades, permitiendo trabajar de forma organizada en el frontend y backend antes de integrarlas en la rama principal.

---

# Tecnologías Utilizadas

## Frontend

* HTML5
* CSS3

## Backend

* Python 3
* Flask

## Contenedores

* Docker
* Docker Compose

## Control de Versiones

* Git
* GitHub

---

# Desarrollo del Proyecto

## Fase 1: Creación del Repositorio Local

Se creó el directorio principal del proyecto y se inicializó Git.

```bash
mkdir festival-devops
cd festival-devops
git init
```

---

## Fase 2: Estructura Inicial

Se definió la estructura base del proyecto:

```text
festival-devops/
├── frontend/
├── backend/
├── docker-compose.yml
└── README.md
```

---

## Fase 3: Primer Commit

Se registró la estructura inicial del proyecto en Git.

```bash
git add .
git commit -m "Estructura inicial del proyecto"
```

---

## Fase 4: Desarrollo de la Landing Page

Se creó una rama específica para el desarrollo del frontend.

```bash
git checkout -b feature-landing
```

Archivos agregados:

```text
index.html
style.css
```

Commit realizado:

```bash
git add .
git commit -m "Se agrega landing page del festival"
```

---

## Fase 5: Desarrollo del Backend

Se creó una rama independiente para la API desarrollada con Flask.

```bash
git checkout -b feature-backend
```

Archivos agregados:

```text
app.py
requirements.txt
Dockerfile
```

Commit realizado:

```bash
git add .
git commit -m "Se agrega API Flask"
```

---

## Fase 6: Integración de Cambios

Se realizó la integración de las ramas de trabajo hacia la rama principal.

```bash
git checkout master
git merge feature-landing
git merge feature-backend
```

Nota: En este proyecto la rama principal se llama **master**, por lo que se utilizó dicho nombre en lugar de **main**.

---

## Fase 7: Creación del Repositorio Remoto

Se creó el repositorio remoto en GitHub:

```text
festival-devops-2026
```

---

## Fase 8: Publicación en GitHub

Se vinculó el repositorio local con GitHub y se publicaron los cambios.

```bash
git remote add origin https://github.com/KevinMarinGallego/festival-devops-2026.git
git push -u origin master
```

---

# Docker

Docker permite empaquetar aplicaciones junto con todas sus dependencias para garantizar que funcionen de manera consistente en cualquier entorno.

Ejemplo de construcción de imagen:

```bash
docker build -t festival-api .
```

Ejemplo de ejecución:

```bash
docker run -p 5000:5000 festival-api
```

---

# Docker Compose

Docker Compose facilita la administración de múltiples contenedores mediante un único archivo de configuración.

Ejemplo:

```bash
docker-compose up -d
```

Para detener los servicios:

```bash
docker-compose down
```

---

# Git y GitHub

## Git

Git es un sistema de control de versiones distribuido que permite registrar cambios en el código fuente y colaborar con otros desarrolladores.

Comandos utilizados:

```bash
git init
git add .
git commit
git checkout
git merge
git push
```

## GitHub

GitHub es una plataforma que permite almacenar repositorios Git en la nube, facilitando la colaboración y el seguimiento de proyectos.

Repositorio del proyecto:

```text
https://github.com/KevinMarinGallego/festival-devops-2026
```

---

# Estructura Final del Proyecto

```text
festival-devops/
├── frontend/
│   ├── index.html
│   └── style.css
│
├── backend/
│   ├── app.py
│   ├── requirements.txt
│   └── Dockerfile
│
├── docker-compose.yml
└── README.md
```

---

# Autor

Kevin Marín Gallego

Proyecto académico desarrollado para la práctica de Git, GitHub, Docker y Docker Compose.
