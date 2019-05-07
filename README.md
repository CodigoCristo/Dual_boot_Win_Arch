Guia rapida de uso de pacman <br>
Sincroniza la base de datos con los repositorios.<br>
pacman -Sy<br>
<br>
Actualiza el sistema completo.<br>
pacman -Syu<br>
pacman -Syyu <br>
para forzar una actualización de todas las listas de paquetes<br>
seguidamente, actualizar el sistema.<br>
<br>
Instala un paquete.<br>
pacman -S Paquete<br>
<br>
Desinstala un paquete.<br>
pacman -R paquete<br>
<br>
Desinstala un paquete junto a las dependencias no utilizadas por otros paquetes.<br>
pacman -Rs paquete<br>
<br>
Permite buscar a un paquete específico<br>
pacman -Ss Paquete<br>
<br>
Descarga el paquete pero no lo instala<br>
pacman -Sw paquete<br>
<br>
Muestra información sobre un paquete no instalado<br>
pacman -Si paquete<br>
<br>
Muestra información sobre un paquete ya instalado<br>
pacman -Qi paquete<br>
<br>
Instala solamente las dependencias del paquete.<br>
pacman -Se paquete<br>
<br>
Muestra todos los archivos pertenecientes al paquete.<br>
pacman -Ql Paquete<br>
<br>
Muestra los paquetes del sistema que pueden ser actualizados, pero no los instala.<br>
pacman -Qu<br>
<br>
Muestra una lista de todos los paquetes instalados en el sistema.<br>
pacman -Q<br>
<br>
Muestra a cual paquete pertenece un archivo en especial.<br>
pacman -Qo /ruta/del/archivo<br>
<br>
Borra todos los paquetes antiguos guardados en la caché de pacman.<br>
pacman -Sc<br>
<br>
Borra todos los paquetes guardados en la cache de pacman ubicado en /var/cache/pacman/pkg.<br>
pacman -Scc<br>
<br>
Instala un paquete guardado en una carpeta local.<br>
pacman -U /ruta/al/paquete/nombre_paquete-versión.pkg.tar.xz<br>
<br>
Eliminación de paquetes no utilizados (huérfanos)<br>
pacman -Rns $(pacman -Qtdq)<br>
<br>
