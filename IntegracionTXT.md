# IntegracionTXT

La integración desde archivos de texto plano se realiza de la siguiente forma.

<b>PROCEDIMIENTO PARA REALIZAR LA INTEGRACIÓN CON ARCHIVO TXT</b>
<br>A) Crear un Archivo Txt
<br>B) Enviar Archivo Txt
<br>C) Recuperar Archivo Xml
<br>D) Cargar Xml en Sistema Propio

<b>A) CREAR ARCHIVO TXT:</b>
<br>A-01.-Generar con su sistema un archivo TXT
<br>A-02.-Desde el siguiente link puede ver un ejemplo del archivo Txt que debe construir
<br>A-03.-Link Archivo txt Timbrar Folios: https://github.com/FacTronica/TimbrarFolios/blob/main/txt_caf.php
<br>A-04.-En el archivo txt se encuentra documentada cada línea con los valores que se deben enviar
<br>A-05.-Como ejemplo utilizaremos la siguiente carpeta y nombre de archivo plano c:\curl\txt_caf.php
<br>A-06.-Es importante señalar que al construir el archivo plano debe comenzar con <?php y finalizar con ?>

<b>B) ENVIAR ARCHIVO TXT:</b>
<br>B-01.-Enviar el archivo txt al servidor de SDK Factronica ( Puede ser al servidor propio o a Servidor Factronica )
<br>B-02.-Para enviar con windows c:\curl\curl.exe --form "archivocaf=@c:\curl\txt_caf.php" http://www.urlservidor.cl/sdk/factronica_timbrardte/recibe_txt.php
<br>B-03.-Para enviar con Linux curl --form "archivocaf=@txt_caf.php" http://www.urlservidor.cl/sdk/factronica_timbrardte/recibe_txt.php

<b>B) RECUPERAR ARCHIVO XML:</b>
<br>B-01.-Recuperar el archivo xml con el comando
<br>B-02.-Para recuperar con windows c:\curl\curl.exe --form "archivocaf=@c:\curl\txt_caf.php" http://www.urlservidor.cl/sdk/factronica_timbrardte/recibe_txt.php
<br>B-03.-Para enviar con Linux curl -o c:\curl\caf.xml http://www.urlservidor.cl/sdk/factronica_timbrardte/caf/caf.xml
<br>B-04.-Al realizar este proceso tendrá elmacenado el archivo xml descargado del sii con los datos del timbraje


<b>D) CARGAR XML EN SISTEMA PROPIO:</b>
<br>B-01.-Desde su sistema leer el archivo xml con el caf
<br>B-02.-Con los datos leidos, debe insertarlos en la base de datos de su sistema propio
<br>B-03.-Al realizar este procedimiento debería tener cargado de forma automatizada los folios caf en su sistema propio


