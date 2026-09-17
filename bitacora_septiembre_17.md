# Bitácora Septiembre - Semana 3 (17/09/2026)
Autora: Jessica Tatiana Serrano Pérez
Ficha: 3381732

## ID 001
- Fecha: 17/09/2026
- Hora: 2:25 PM - 2:35 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Lectura del esquema de ramas dibujado en el tablero por el instructor. Elementos identificados: línea superior "Main", línea intermedia "Develop" y línea inferior "Feature/nombre"; cada círculo con X representa un commit; las líneas del extremo derecho unen feature -> develop -> main (fusiones); el 1 marca git init como primer paso.
- Impedimentos: Sin impedimentos operativos.
- Plan: Verificar la versión de Git y configurar la identidad del usuario en la terminal.

## ID 002
- Fecha: 17/09/2026
- Hora: 2:35 PM - 2:40 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Consulta de la versión instalada de Git (2.55.0.windows.5) y configuración global del nombre y del correo que Git asocia a cada commit.
- Comandos ejecutados:
  git --version
  git config --global user.name "Jessica Serrano"
  git config --global user.email "jtserranop6@gmail.com"
- Impedimentos: Sin impedimentos operativos.
- Plan: Ubicar la unidad D: y la carpeta de trabajo adso.

## ID 003
- Fecha: 17/09/2026
- Hora: 2:40 PM - 2:46 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Cambio a la unidad D: y listado de su contenido para identificar la carpeta adso.
- Comandos ejecutados:
  cd D:
  ls
- Impedimentos: Sin impedimentos operativos.
- Plan: Entrar a /d/adso y crear la carpeta del ejercicio.

## ID 004
- Fecha: 17/09/2026
- Hora: 2:46 PM - 2:53 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Ingreso a /d/adso y a la subcarpeta 3381732 (el prompt muestra la rama (main), por lo que esa carpeta ya era un repositorio); regreso a /d/adso, creación del directorio pasado-y-presente, listado de verificación e ingreso al directorio.
- Comandos ejecutados:
  cd adso
  cd 3381732
  cd ..
  mkdir pasado-y-presente
  ls
  cd pasado-y-presente
- Impedimentos: Sin impedimentos operativos.
- Plan: Inicializar el repositorio dentro de pasado-y-presente.

## ID 005
- Fecha: 17/09/2026
- Hora: 2:53 PM - 3:00 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Inicialización del repositorio en D:/ADSO/pasado-y-presente/.git/. Creación de README.md con el título del proyecto y primer commit (root-commit e6524fc) en la rama main.
- Comandos ejecutados:
  git init
  echo "# Pasado y Presente" > README.md
  git add .
  git commit -m "commit 1: inicial en main"
- Evidencia: Captura de terminal Git Bash - trabajo_jessica_serrano.docx
- Impedimentos: Sin impedimentos operativos. Git emitió la advertencia informativa "LF will be replaced by CRLF" al ejecutar git add; no interrumpió el comando.
- Plan: Crear la rama develop a partir de main.
