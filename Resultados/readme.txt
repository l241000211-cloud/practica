
Resultados Esperados vs. Resultados Obtenidos
En esta práctica se evaluó el comportamiento de la terminal de Ubuntu frente a diferentes comandos de navegación, listado y administración de privilegios.

1. Comandos de Listado (ls)
ls

Resultado esperado: Despliegue de nombres de carpetas y archivos visibles en columnas horizontales.

Resultado obtenido: Se listaron correctamente los elementos del directorio actual clasificados por colores (azul para carpetas y blanco para archivos estándar).

ls -l

Resultado esperado: Formato de lista detallada con permisos, enlaces, usuario, grupo, tamaño en bytes y fecha.

Resultado obtenido: Se desplegó la tabla con los permisos en notación drwxr-xr-x, confirmando la pertenencia de los archivos al usuario actual y mostrando tamaños en bytes exactos.

ls -la

Resultado esperado: Inclusión de archivos y carpetas ocultas del sistema.

Resultado obtenido: Se visualizaron los archivos de configuración que inician con un punto (como .bashrc, .profile y los directorios de navegación . y ..).

ls -lh

Resultado esperado: Visualización de tamaños de archivo con unidades simplificadas.

Resultado obtenido: La columna de peso sustituyó los bytes extensos por unidades legibles como 4.0K, facilitando la lectura del espacio ocupado.

2. Comandos de Navegación (cd)
cd Descargas

Resultado esperado: Cambio de directorio hacia la subcarpeta indicada sin mensajes de confirmación.

Resultado obtenido: El prompt de la terminal actualizó exitosamente la ruta activa de ~$ a ~/Descargas$.

cd ..

Resultado esperado: Retorno de un nivel en la jerarquía hacia el directorio padre.

Resultado obtenido: La ruta regresó de forma inmediata a la carpeta personal (~$).

cd ~ / cd

Resultado esperado: Regreso directo al directorio raíz del usuario sin importar la profundidad de navegación.

Resultado obtenido: Retorno comprobado a /home/israel.

3. Ejecución con Privilegios (sudo)
sudo ls

Resultado esperado: Solicitud de credenciales de seguridad y ejecución de la orden con privilegios de superusuario (root).

Resultado obtenido: La terminal solicitó la contraseña de usuario mediante un método de entrada oculta (sin eco de caracteres ni asteriscos en pantalla). Al validarla, ejecutó la orden con permisos elevados de manera transparente.
