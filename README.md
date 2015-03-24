# Openldap-wrapper


Este proyecto es un adapter de la [openLDAP Library](http://www.openldap.org) exclusivamente realizado para la cátedra de Sistemas Operativos de FRBA UTN.


>  Al codigo no está finalizado por ende puede contener errores
>  en el diseño y de programación ya que como es a modo de ejemplo
>  no se tuvieron en cuenta cuestiones de memoria.


## Contenido del paquete:

|Archivo|Descripción|
|:------|:----------|
|`Ldap.c`|código de ejemplo|
|`LdapWrapper.c`|definición de las funciones de la API|
|`LdapWrapper.h`|declaración de la API|
|`ldap_wrapper_tutorial.pdf`|Tutorial explicativo de como utilizar la API|
|`lib`|openLDAP dynamic link libraries|
|`include`|openLDAP headers|


## Compilación

``` console
$ tar -zxvf openLdap-wrapper-0.1.tar.gz
$ cd openLdap-wrapper-0.1/
$ gcc -o ldap-test Ldap.c LdapWrapper.c -Iinclude -Llib -lldap -llber
```

## Requesitos minimos
El sistema deberá tener instalado las development libraries de [OpenLDAP](http://www.openldap.org). En Debian fueron testeadas usando la versión **libldap-2.4**.