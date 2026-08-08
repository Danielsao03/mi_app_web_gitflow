# 🚀 Formulario Contacto — Git Flow Practice

Un proyecto web ultra sencillo desarrollado con el propósito principal de poner en práctica la metodología y el flujo de trabajo con **Git Flow**.

---

## 🎯 Objetivo del Proyecto

La aplicación es un formulario minimalista que recibe un nombre y un correo electrónico para renderizarlos dinámicamente en pantalla al enviar. 

El foco principal de este repositorio **no es la complejidad del código**, sino la adopción de buenas prácticas de control de versiones:
* Manejo del ciclo de vida con ramas `main` y `develop`.
* Aislamiento de tareas mediante ramas `feature/`.
* Versionado semántico a través de `release/`.
* Tambien el uso de ramas `hotfix/`.


## 🌿 Flujo de Git Practicado

Durante el desarrollo de este mini proyecto se aplicaron los siguientes comandos e hitos de Git Flow:

```bash
# Inicialización del flujo
git flow init

# Creación de ramas de funcionalidades
git flow feature start formulario-contacto
git commit -m "Añadir formulario de contacto" 
git flow feature finish formulario-contacto

# Preparación y cierre del lanzamiento v1.0.0
git flow release start v1.0.0
git commit -m "Preparar version v1.0.0" 
git flow release finish v1.0.0
git push origin develop
git push origin main --tags   

# Simulación de error para uso de rama "hotfix"
git flow hotfix start v1.0.1
git commit -m "Corregir error crítico" 
git flow hotfix finish v1.0.1
git push origin develop
git push origin main --tags   




