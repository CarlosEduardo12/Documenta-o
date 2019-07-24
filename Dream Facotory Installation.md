# Como instalar DreamFactory clonando o repositorio em ambiente Windows
O DreamFactory é um software livre, Backend de API REST para aplicativos móveis, da Web e IoT. Ele é construído sobre o framework Laravel e inclui um cliente de administração web orientado por AngularJS.

[GitHub DreamFactory](https://github.com/dreamfactorysoftware/dreamfactory)

#### .env
Editar o .env com as informações de banco e demais informações.

## Dependências
Utilizaremos o [WAMP](http://www.wampserver.com/en/) como um conjunto de softwares que engloba tudo que precisamos para executar o DF 

### Dependências extra para o PHP

#### MongoDB
Para instalar essa dependência basta escolher a versão do PHP que o WAMP esta utilizando e baixar o pacote com a dll no [link](https://pecl.php.net/package/mongodb/1.5.5/windows)

* Adicionar o .dll no diretorio do PHP no WAMP _C:\wamp64\bin\php\phpx.x.x\ext_
* Adicionar a extensão no php.ini
* Reiniciar todos os serviços do WAMP

#### OCI8
Para instalar essa dependência basta escolher a versão mais recente e baixar o pacote com a dll no [link](https://pecl.php.net/package/oci8)

* Adicionar o .dll no diretorio do PHP no WAMP _C:\wamp64\bin\php\phpx.x.x\ext_
* Adicionar/descomentar a extensão no php.ini
* Baixar o cliente no site da [Oracle](https://www.oracle.com/database/technologies/instant*client/downloads.html) (Recomendação versao 10)
* Criar um diretorio na raiz
 - Ex: C:\Oracle\instantclient_10_2
* Criar as variaveis de ambiente e adicionar no Path. Ex: 
 - OCI_LIB64 :  C:\oracle\instantclient_10_2 
 - TNS_ADMIN :  C:\oracle\instantclient_10_2

* Reiniciar todos os serviços do WAMP
