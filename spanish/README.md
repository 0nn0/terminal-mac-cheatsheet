# Terminal Cheatsheet para Mac (básico)

_Las letras se muestran en mayúsculas solo para facilitar la lectura. Capslock debería estar desactivado._

## ATAJOS

| Atajo | Descripción |
| ------ | ----------|
| Ctrl + A | Ir al inicio de la linea en la que se esta escribiendo |
| Ctrl + E | Ir al final de la linea en la que se esta escribiendo |
| Ctrl + L | Limpa a pantalla |
| Command + K | Limpa a pantalla |
| Ctrl + U | Corta todo el contenido hasta el inicio de la linea a partir de la posicion del cursor |
| Ctrl + K | Corta todo el contenido hasta el final de la linea a partir de la posicion del cursor |
| Ctrl + W | Corta una palabra anterior a la posicion del cursor usando el espacio como delimitador |
| Ctrl + Y | Pega el contenido cortado por el ultimo comando de corte anterior |
| Ctrl + H | Igual que backspace |
| Ctrl + C | Termina cualquier proceso ejecutadose y borra el contenido de la linea actual |
| Ctrl + D | Salir de la shell actual cuando no se este ejecutando ningun proceso o enviar EOF al proceso en ejecucion |
| Ctrl + Z | Coloca cualquier proceso en ejecución en un proceso en segundo plano. El comando "fg" lo restaura. |
| Ctrl + _ | Deshace el ultimo comando, (Guión bajo es ctualmente Ctrl + Shift + Guión) |
| Ctrl + T | Intercambia las dos ultimas legras antes del cursor |
| Ctrl + F | Mueve el cursor un caracter hacia adelante |
| Ctrl + B | Mueve el cursor un caracter hacia atras |
| Option + → | Mueve el cursor una palabra hacia adelante |
| Option + ← | Mueve el cursor una palabra hacia atras |
| Esc + T | Intercambia las dos ultimas palabras antes del cursor |
| Esc + Backspace | Corta una palabra anterior a la posicion del cursor usando caracteres no alfabeticos como delimitador |
| Tab | Autocompletar |

## COMANDOS PRINCIPALES

| Comando | Descripción |
| ------ | ----------|
| cd [folder] | Cambiar de directorio |
| cd | Ir al directorio principal |
| cd ~ | Ir al directorio principal |
| cd / | Ir al directorio raiz |
| cd - | Ir al directorio anterior |
| ls | Listado corto de archivos |
| ls -l | Listado largo de archivos |
| ls -a | Listado incluyendo archivos ocultos |
| ls -lh | Listado largo de archivos con tamaño de archivos legibles para humanos |
| ls -R | Todo el contenido de la carpeta recursivamente |
| sudo [command] | Ejecuta un comando con privilegios de super usuario |
| open [file] | Abre un archivo ( Como si hicieras doble click sobre el ) |
| top | Muestra los procesos activos, presiona q para salir |
| nano [file] | Abre un archivo usando el editor nano |
| vim [file] | Abre un archivo usando el editor vim |
| clear | Limpia la pantalla |
| reset | Restablece la pantalla del terminal |

## ENCADENAMIENTO DE COMANDOS

| Tecla / Comando | Descripción |
| ------ | ----------|
| [command-a]; [command-b] | Ejecutar el comando A y luego B, independientemente del éxito de A |
| [command-a] && [command-b] | Ejecutar el comando B si A tuvo éxito |
| [command-a] || [command-b] | Ejecutar el comando B si A falló |
| [command-a] & | Ejecutar el comando A en segundo plano |

## CANALIZANDO COMANDOS

| Tecla / Comando | Descripción |
| ------ | ----------|
| [command-a] | [command-b] | Ejecutar el comando A y luego pasar el resultado al comando B, por ejemplo, ps auxwww | grep google |

## HISTORIAL DE COMANDOS

| Tecla / Comando | Descripción |
| ------ | ----------|
| history n | Muestra el historial: agregue un número para limitar los últimos n elementos |
| Ctrl + r | Búsqueda interactiva a través de comandos previamente escritos |
| ![value] | Ejecute el último comando escrito que comienza con 'value' |
| ![value]:p | Imprima en la consola el último comando escrito que comienza con 'value' |
| !! | Ejecutar el último comando escrito. |
| !!:p | Imprimir en la consola el último comando escrito. |

## GESTIÓN DE ARCHIVOS

| Tecla / Comando | Descripción |
| ------ | ----------|
| touch [file] | Crear un nuevo archivo |
| pwd | Ruta completa del directorio actual |
| . | Carpeta actual, por ejemplo `ls .` |
| .. | Carpeta anterior, por ejemplo `ls ..` |
| ls -l .. | Listado largo de archivos de la carpeta anterior |
| cd ../../ | Mover 2 niveles hacia arriba |
| cat | Mostrar en pantalla el contenido de un archivo |
| rm [file] | Eliminar un archivo, por ejemplo `rm data.tmp` |
| rm -i [file] | Eliminar un archivo con solicitud de confirmación |
| rm -r [dir] | Eliminar un directorio y su contenido |
| rm -f [file] | Eliminar un directorio y su contenido |
| rm -r [dir] | Forzar eliminado sin solicitar confirmacion |
| rm -f [file] | Eliminar un directorio y su contenido |
| cp [file] [newfile] | Copiar file a newfile |
| cp [file] [dir] | Copiar el archivo al directorio |
| mv [file] [new filename] | Mover / Renombrar, ejemplo `mv file1.ad /tmp` |
| pbcopy < [file] | Copia el contenido del archivo al portapapeles. |
| pbpaste | Pegar contenido del portapapeles |
| pbpaste > [file] | Pegue el contenido del portapapeles en un archivo |

## GESTIÓN DE DIRECTORIOS

| Tecla / Comando | Descripción |
| ------ | ----------|
| mkdir [dir] | Crear un nuevo directorio |
| mkdir -p [dir]/[dir] | Crear directorios anidados |
| rmdir [dir] | Eliminar directorio (solo funciona en directorios vacíos) |
| rm -R [dir] | Eliminar el directorio y su contenido |
| less [file] | Contenido del archivo entregado en trozos de tamaño de pantalla |
| [command] > [file] | Envia la salida al archivo, tenga en cuenta que se sobrescribirá el contenido |
| [command] >> [file] | Añadir salida al archivo existente |
| [command] < [file] | Indicar al comando leer el contenido de un archivo |

## BUSCAR

| Tecla / Comando | Descripción |
| ------ | ----------|
| find [dir] -name [search_pattern] | Buscar archivos por nombre, por ejemplo `find /Users -name "archivo.txt"`. |
| grep [search_pattern] [file] | Busque todas las líneas que contienen el patrón `search_pattern` en su contenido, por ejemplo, `grep "Tom" archivo.txt`. |
| grep -r [search_pattern] [dir] | Busque recursivamente en todos los archivos en el directorio especificado para todas las líneas que contienen el patrón `search_pattern`. |
| grep -v [search_pattern] [file] | Busca todas las líneas que NO contienen el patrón `search_pattern`. |
| grep -i [search_pattern] [file] | Busque todas las líneas que contienen el patrón `search_pattern` que distingue entre mayúsculas y minúsculas. |
| mdfind [search_pattern] | Búsqueda destacada de archivos (nombres, contenido, otros metadatos), por ejemplo `mdfind skateboard`. |
| mdfind -onlyin [dir] -name [pattern] | Spotlight busca archivos nombrados como patrón `search_pattern` en el directorio dado. |

## AYUDA

| Tecla / Comando | Descripción |
| ------ | ----------|
| [command] -h | Mostrar la ayuda del comando |
| [command] --help | Mostrar la ayuda del comando |
| info [command] | Mostrar la ayuda del comando |
| man [command] | Muestra el manual de ayuda del comando |
| whatis [command] | Da una descripción de una línea del comando |
| apropos [search-pattern] | Busca comandos con palabras clave en la descripción. |