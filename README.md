# php-CLI

Forma de utilizar o PHP 7.2.11, composer e laravel, sem necessidade de instalação uma forma simples de montar um ambiente mesmo sem privilégios de instalação


Realizar o Download

#### PHP 7.2.11[x64](https://windows.php.net/downloads/releases/php-7.2.11-nts-Win32-VC15-x64.zip)

#### PHP 7.2.11[x86](https://windows.php.net/downloads/releases/php-7.2.11-nts-Win32-VC15-x86.zip)

Renomear o arquivo para php-7.2.11

## Comandos para download 
```sh
$ wget -O php-7.2.11.zip https://windows.php.net/downloads/releases/php-7.2.11-nts-Win32-VC15-x64.zip --progress=bar:force
```
Descompactar no diretorio utilizando o nome php-7.2.11

```sh
$ unzip php-7.2.11.zip -d php
```
Criar arquivo para informar versão 
(echo phpinfo();) | php > PHP-7.2.11.txt

copiar arquivo php.ini-development
```sh
$ cp php.ini-development php.ini
```
Editar o arquivo de Configuração do php 
*php.ini*

Descomentar estas extensões para uso

```sh
extension_dir = "ext"

extension=curl
extension=fileinfo
extension=mbstring
extension=mysqli
extension=openssl
extension=pdo_mysql
extension=pdo_sqlite
```

testar utilizado o comando 
```sh
$ php -v
$ php -r phpinfo();
$ echo criar um arquivo para saber a versão
$ php -i > Version_php-7.2.11.txt
```

definir o php para uso
```sh
$ EXPORT PATH=$PATH:'/c/web/php'
```

definir o caminho para o composer
```sh
$ EXPORT PATH=$PATH:'/c/web/composer/bin' 
```

definir o caminho para o laravel
```sh
$ EXPORT PATH=$PATH:'/c/web/laravel/vendor/bin' 
```

Comando para fazer backup
```sh
@XCOPY c:\Temp\*.* D:\c\Temp /D /E /Y /C /K >> logbackup.txt
```
