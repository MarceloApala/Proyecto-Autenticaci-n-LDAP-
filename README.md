# **Proyecto de Autenticación con Active Directory/OpenLDAP**

Este proyecto es una implementación de autenticación utilizando **Active Directory** o **OpenLDAP** mediante la librería **LDAPRecord**. El propósito de esta aplicación es facilitar la integración de servicios de autenticación en sistemas que requieren la validación de usuarios a través de LDAP, permitiendo la gestión centralizada de las credenciales de acceso.

## Descripción

Este proyecto proporciona un sistema de autenticación basado en **LDAP** (Active Directory o OpenLDAP) que permite a los usuarios autenticarse de manera segura utilizando sus credenciales almacenadas en un servidor LDAP. El proyecto utiliza la librería **LDAPRecord** para facilitar la comunicación con el servidor LDAP, realizar la validación de credenciales y gestionar la autenticación de los usuarios.

### Funcionalidades

- **Autenticación con Active Directory**: Valida las credenciales de los usuarios contra un servidor **Active Directory**.
- **Autenticación con OpenLDAP**: Valida las credenciales de los usuarios contra un servidor **OpenLDAP**.
- **Autenticación segura**: Se asegura de que la comunicación con el servidor LDAP esté cifrada.
- **Gestión de usuarios**: Permite la validación de usuarios, así como la recuperación de información adicional, como el nombre completo, el correo electrónico y los grupos a los que pertenece el usuario.
- **Compatibilidad con múltiples servidores LDAP**: Configuración flexible para conectar con diferentes instancias de LDAP.

## Tecnologías y Librerías Utilizadas

- **Laravel**: Framework PHP utilizado para la construcción de la aplicación.
- **LDAPRecord**: Paquete para interactuar con servidores LDAP, permitiendo la autenticación y la gestión de usuarios.
- **PHP**: Lenguaje de programación utilizado en el proyecto.
- **Composer**: Herramienta de gestión de dependencias para PHP.

## Requisitos previos

Asegúrate de tener instalados los siguientes programas antes de comenzar con la instalación:

1. **PHP**: Recomendado PHP 7.4 o superior. Puedes descargarlo desde [aquí](https://www.php.net/downloads.php).
2. **Composer**: Puedes instalar Composer desde [su página oficial](https://getcomposer.org/).
3. **Servidor LDAP**: Active Directory o OpenLDAP funcionando y accesible desde tu aplicación.

## Instalación y Configuración

### 1. Instalar dependencias

composer install

### 1. Configuración de LDAP

LDAP_CONNECTION=ldap
LDAP_HOST=ldap://tu-servidor-ldap.com
LDAP_PORT=389
LDAP_USERNAME=cn=admin,dc=ejemplo,dc=com
LDAP_PASSWORD=tu-contraseña
LDAP_BASE_DN=dc=ejemplo,dc=com
LDAP_ADMIN_GROUP=cn=admins,dc=ejemplo,dc=com

### 3. Ejecutar la aplicación

php artisan serve


