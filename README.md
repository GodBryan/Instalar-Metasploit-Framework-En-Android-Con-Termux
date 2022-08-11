# Instalar-Metasploit-Framework-En-Android-Con-Termux

![images](https://user-images.githubusercontent.com/90482037/184072227-0006aea2-038c-4cbb-8343-89d898478f07.png)

Metasploit es un proyecto de código abierto para la seguridad informática, que proporciona información acerca de vulnerabilidades de seguridad y ayuda en tests de penetración "Pentesting" y el desarrollo de firmas para sistemas de detección de intrusos. Wikipedia

Antes de comenzar, quiero decirles que NO SE NECESITA ROOT.
Bien, comenzamos instalando Termux como anteriormente hablamos de termux y como descargar + los comandos que deberíamos aprender .
Requisitos
1) Android 5.0 en adelante
2) Termux ( Descárguelo de Google Play o Play Store )
3). Alrededor de 500 mb de almacenamiento interno ( para la instalación adecuada de Metasploit )
Una vez descargado la app de termux , instale desde Google Play o descargue el último archivo APK desde AQUÍ .
https://play.google.com/store/apps/details?id=com.termux&hl=en
https://termux.en.uptodown.com/android

✫Lo que aremos antes de instalar cualquier paquete (script,freimork,etc) vamos a actualizar con el comando .
$pkg upgrate 

✫Luego instalaremos los programas que requerimos para instalar el freimork de metasploits  serán wget o curl
$pkg update && pkg upgrade -y && pkg install wget curl openssh git -y
ó
$pkg install curl
$pkg install wget

![1](https://user-images.githubusercontent.com/90482037/184072298-7aa9ae42-7208-4ad9-a42a-42c94d19add6.jpg)

(Espere hasta que esté completamente instalado)
✫Ahora, tendremos que poner para descargar Metasploit
$curl -LO https://raw.githubusercontent.com/Hax4us/Metasploit_termux/master/metasploit.sh
ó
$wget https://raw.githubusercontent.com/Hax4us/Metasploit_termux/master/metasploit.sh

![2](https://user-images.githubusercontent.com/90482037/184072368-ce1b0e71-0198-4679-ab9d-5072e8ae01fc.jpg)

✫Aquí les dejo la URL https://raw.githubusercontent.com/Hax4us/Metasploit_termux/master/metasploit.sh

✫Le daremos permisos al instalador de Metasploit
$chmod 777 metasploit.sh
ó
$chmod +x metasploit.sh
ó
$chmod +x metasploit.sh && ./metasploit.sh
✫Cualquiera de las lineas de comando pueden usar para darle permiso y que se instale
Si observamos una linea en termux de color verde significara que se instalo correctamente
$./metasploit.sh

✫Usamos el comando para limpiar
$clear
y luego el comando para ver el directorio y saber si existe la carpeta metasploit-framework
$ls
✫Luego insgresamos a la carpeta metasploit-framework
$cd metasploit-framework

![4](https://user-images.githubusercontent.com/90482037/184072464-239611af-5ebc-426a-8702-7bb1cbc2c6fa.jpg)

Listo para usar metasploit en nuestro android
$./msfconsole

![5](https://user-images.githubusercontent.com/90482037/184072539-f030176f-6f76-4baa-aa4f-ec98c0997c15.jpg)

✫Aquí te dejo los comandos ordenados + otros métodos para instalar termux la idea del blog es que sepan como funciona la instalación . :)

Primer Método
$pkg upgrade
$pkg install curl
$curl -LO https://raw.githubusercontent.com/Hax4us/Metasploit_termux/master/metasploit.sh
$chmod 777 metasploit.sh
$./metasploit.sh
$clear
$cd metasploit-framework
$ls
$./msfconsole

Segundo Método
$pkg upgrade
$pkg install curl
$curl -LO https://raw.githubusercontent.com/Hax4us/Metasploit_termux/master/metasploit.sh
$chmod +x metasploit.sh
$clear
$cd metasploit -framework
$ls
$chmod +x msfconsole
$msfconsole

Tercer Método 
$pkg upgrade
$pkg install wget
$wget https://raw.githubusercontent.com/Hax4us/Metasploit_termux/master/metasploit.sh
$clear
$ls
$chmod +x metasploit.sh && ./metasploit.sh

Cuarto Método 
$pkg update && pkg upgrade -y && pkg install curl wget tsu wget git && wget https://raw.githubusercontent.com/Hax4us/Metasploit_termux/master/metasploit.sh && bash metasploit.sh

Quinto Método "verluchie"
$pkg update && pkg upgrade && pkg install curl wget git && git clone github.com/verluchie/termux-metasploit && chmod 777 termux-metasploit/install.sh && sh termux-metasploit/install.sh

Sexto Método
$apt update && apt upgrade && apt install curl && curl -LO https://raw.githubusercontent.com/Hax4us/Metasploit_termux/master/metasploit.sh && chmod 777 metasploit.sh && sh metasploit.sh
