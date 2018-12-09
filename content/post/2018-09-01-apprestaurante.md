---
date: "2018-09-01"
title: "APP Restaurante"
description: "En estas oportunidad les presento un nuevo sistema de restaurante, cuenta con dos formas de ver, una para los pedidos que se configura dentro del sistema y la otra la parte administrativa."
author: "Hugo Roca"
image: /images/post/apprestaurante.jpg
tags:
 - SQLSERVER
 - CSharp
 - JS
 - JQUERY
categories:
 - JavaScript
 - C Sharp
 - Sistemas
---

En estas oportunidad les presento un nuevo sistema de restaurante, cuenta con dos formas de ver, una para los pedidos que se configura dentro del sistema y la otra la parte administrativa.

### Contenido
- Registro del menú del día 
- Registro de empleados 
- Control de acceso de usuario 
- Cobranza 
- Genera PDF del Cobro 
- Registro de imagenes 
- Vista rápida en dashboard 

## Paso 1
Puedes obtener el codigo fuente de la siguiente forma:

1. Clonar [APPRESTAURANTE](https://github.com/PORTAFOLIO-PROYECTOS/APPRESTAURANTE)
2. Abrir Visual Studio
3. Buscar la solución y abrir
4. Tambien puedes hacer 'FORK' y abrirlo directo de GitHub

## Paso 2
Ejecutar el script de base de datos ```DataBase/APPRestaurente.sql``` en SQLServer.

## Paso 3
Configurar el archivo ```App/Portafolio.Web/Web.config```
```
<!-- 
Si tienes configurado el sqlserver con windows autentication solo debes de 
cambiar el data source por => "."; En caso que tenga un usuario y contraseña 
solamente agregarlo
-->
<connectionStrings>
    <add name="PortafolioContext" 
        connectionString="
            data source=HUGOROCA;
            initial catalog=portafolio;
            integrated security=True;
            MultipleActiveResultSets=True;
            App=EntityFramework" 
        providerName="System.Data.SqlClient" />
</connectionStrings>
```

## Paso 4
Ejecutar el proyecto, para acceder al administrador solamente debes de agregar a la URL "/Admin"

```
Ejemplo: http://localhost:666/admin
```

Comenta, disfruta y comparte! 
