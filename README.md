# php-CLI

Forma de utilizar o PHP 7.2.11, composer e laravel, sem necessidade de instalação uma forma simples de montar um ambiente mesmo sem privilégios de instalação


Realizar o Download do *PHP 7.2.11*
[x64](https://windows.php.net/downloads/releases/php-7.2.11-nts-Win32-VC15-x64.zip)
[x86](https://windows.php.net/downloads/releases/php-7.2.11-nts-Win32-VC15-x86.zip)

Renomear o arquivo para php-7.2.11

## Comandos para download 

  $wget -O php-7.2.11.zip https://windows.php.net/downloads/releases/php-7.2.11-nts-Win32-VC15-x64.zip --progress=bar:force

Descompactar no diretorio utilizando o nome php-7.2.11

 $unzip php-7.2.11.zip -d Documents/php

Criar arquivo para informar versão 
(echo phpinfo();) | php > PHP-7.2.11.txt



copiar arquivo php.ini-development
$cp php.ini-development php.ini

Editar o arquivo de Configuração do php 
*php.ini*

Descomentar estas extensões para uso

extension=curl
extension=fileinfo
extension=mbstring
extension=mysqli
extension=openssl
extension=pdo_mysql
extension=pdo_sqlite


definir o php para uso
EXPORT PATH=$PATH:'/c/web/php'

definir o caminho para o composer
EXPORT PATH=$PATH:'/c/web/composer' 

definir o caminho para o laravel
EXPORT PATH=$PATH:'/c/web/laravel' 
