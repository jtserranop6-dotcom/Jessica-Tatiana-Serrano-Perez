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

## ID 006
- Fecha: 17/09/2026
- Hora: 3:00 PM - 3:08 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Creación de la rama develop y cambio a ella con checkout -b. Creación del archivo develop.js y commit 42c8da6 en develop.
- Comandos ejecutados:
  git checkout -b develop
  echo "console.log('develop iniciado');" > develop.js
  git add .
  git commit -m "commit 2: inicial en develop"
- Impedimentos: Sin impedimentos operativos. Git emitió la advertencia informativa "LF will be replaced by CRLF" al ejecutar git add; no interrumpió el comando.
- Plan: Crear la rama feature/nombre desde develop.

## ID 007
- Fecha: 17/09/2026
- Hora: 3:08 PM - 3:16 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Creación de la rama feature/nombre desde develop. Creación del archivo feature.js y commit 3df1265 en feature/nombre.
- Comandos ejecutados:
  git checkout -b feature/nombre
  echo "console.log('feature iniciada');" > feature.js
  git add .
  git commit -m "commit 3: inicial en feature/nombre"
- Impedimentos: Sin impedimentos operativos. Git emitió la advertencia informativa "LF will be replaced by CRLF" al ejecutar git add; no interrumpió el comando.
- Plan: Agregar un segundo commit en feature/nombre.

## ID 008
- Fecha: 17/09/2026
- Hora: 3:16 PM - 3:22 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Adición de una línea a feature.js con el operador >> (agrega sin sobrescribir) y commit 904d6b5 en feature/nombre.
- Comandos ejecutados:
  echo "console.log('mas trabajo en feature');" >> feature.js
  git add .
  git commit -m "commit 4: mas trabajo en feature"
- Impedimentos: Sin impedimentos operativos. Git emitió la advertencia informativa "LF will be replaced by CRLF" al ejecutar git add; no interrumpió el comando.
- Plan: Cambiar a develop y registrar un commit propio de esa rama.

## ID 009
- Fecha: 17/09/2026
- Hora: 3:22 PM - 3:30 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Cambio a develop con git checkout, adición de una línea a develop.js y commit 16bc944. Con este commit develop y feature/nombre quedan en líneas de historial distintas.
- Comandos ejecutados:
  git checkout develop
  echo "console.log('mas trabajo en develop');" >> develop.js
  git add .
  git commit -m "commit 5: mas trabajo en develop"
- Impedimentos: Sin impedimentos operativos. Git emitió la advertencia informativa "LF will be replaced by CRLF" al ejecutar git add; no interrumpió el comando.
- Plan: Cambiar a main y registrar un commit en esa rama.

## ID 010
- Fecha: 17/09/2026
- Hora: 3:30 PM - 3:38 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Cambio a main, adición de una línea a README.md y commit ec57c8f. Las tres ramas tienen commits que las otras no contienen.
- Comandos ejecutados:
  git checkout main
  echo "console.log('mas trabajo en main');" >> README.md
  git add .
  git commit -m "commit 6: mas trabajo en main"
- Impedimentos: Sin impedimentos operativos. Git emitió la advertencia informativa "LF will be replaced by CRLF" al ejecutar git add; no interrumpió el comando.
- Plan: Consultar el historial gráfico de todas las ramas.

## ID 011
- Fecha: 17/09/2026
- Hora: 3:38 PM - 3:45 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Consulta del historial de todas las ramas en formato de grafo. Resultado: main en ec57c8f (HEAD), develop en 16bc944 y feature/nombre en 904d6b5; develop y feature/nombre salen del commit 42c8da6 y main continúa desde e6524fc.
- Comandos ejecutados:
  git log --oneline --graph --all
- Impedimentos: Sin impedimentos operativos.
- Plan: Obtener el hash del primer commit para recuperar README.md de esa versión.

## ID 012
- Fecha: 17/09/2026
- Hora: 3:45 PM - 3:52 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Almacenamiento en la variable HASH_VIEJO del hash del commit más antiguo: git log --oneline lista del más reciente al más antiguo, tail -1 toma la última línea y awk imprime su primer campo. Valor obtenido: e6524fc.
- Comandos ejecutados:
  HASH_VIEJO=$(git log --oneline | tail -1 | awk '{print $1}')
  echo "Trayendo README.md desde el commit: $HASH_VIEJO"
- Impedimentos: Sin impedimentos operativos.
- Plan: Restaurar README.md desde ese commit y registrar el cambio.

## ID 013
- Fecha: 17/09/2026
- Hora: 3:52 PM - 4:00 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Restauración de README.md a la versión del commit e6524fc dentro de main (descarta la línea agregada en el commit 6) y commit dce17ce (1 archivo modificado, 1 línea eliminada).
- Comandos ejecutados:
  git checkout $HASH_VIEJO -- README.md
  git add README.md
  git commit -m "fix: traer README.md del pasado al presente"
- Impedimentos: Sin impedimentos operativos.
- Plan: Confirmar el contenido de README.md y revisar el historial.

## ID 014
- Fecha: 17/09/2026
- Hora: 4:00 PM - 4:08 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Verificación: README.md contiene únicamente "# Pasado y Presente". El grafo muestra dce17ce (HEAD -> main) sobre ec57c8f; develop y feature/nombre aún no están fusionadas en main.
- Comandos ejecutados:
  cat README.md
  git log --oneline --graph --all
- Impedimentos: Sin impedimentos operativos.
- Plan: Fusionar feature/nombre en develop, tal como indica el diagrama del tablero.

## ID 015
- Fecha: 17/09/2026
- Hora: 4:08 PM - 4:18 PM
- Autora: Jessica Tatiana Serrano Pérez
- Actividad: Complemento del flujo del tablero (feature -> develop). Cambio a develop y fusión de feature/nombre. Como develop avanzó con su commit 5 después de crear la rama feature, Git generó el merge commit 53b5fe6 (estrategia ort) en lugar de fast-forward; se incorporó feature.js (2 líneas).
- Comandos ejecutados:
  git checkout develop
  git merge feature/nombre -m "merge: integrar feature/nombre en develop"
  git log --oneline --graph --all
- Impedimentos: Sin impedimentos operativos. No hubo conflictos: cada rama modificó archivos distintos (develop.js y feature.js).
- Plan: Fusionar develop en main.
