---
layout: post
title:  Symfony generator bundle para MongoDB
description: Introducción al GeneratorBundle para MongoDB
name: IsmaAmbrosiGeneratorBundle
categories: [symfony, bundle]
tags: [symfony, bundle, mongodb, generator]
---

[_IsmaAmbrosiGeneratorBundle_][repo] es una extensión del bundle [SensioGeneratorBundle](https://github.com/sensiolabs/SensioGeneratorBundle) para aplicaciones [Symfony](http://symfony.com) que permite generar _documentos_, _formularios_ y controladores _CRUD_ para gestionar esos documentos de MongoDB.

_El bundle SensioGeneratorBundle viene incluido por defecto en la versión standard del framework Symfony. Puedes encontrar más información en su [documentación oficial](http://symfony.com/doc/master/bundles/SensioGeneratorBundle/index.html)._

Proporciona comandos interactivos que permiten generar código, con la ayuda de la librería [mongodb-odm](https://github.com/doctrine/mongodb-odm) de Doctrine.

He estado trabajando en este bundle desde hace unos años pero no se porqué, nunca lo anuncié en ningún lado. Debería haberlo hecho hace un tiempo largo.

Todo surgió cuando trabajaba en ServerGrove, donde se utilizaba MongoDB como motor de base de datos principal... y era genial. Symfony2 recién estaba apareciendo, su versión estable todavía no había sido publicada, pero a nosotros nos funcionaba muy bien.

El problema era que no existía un generador de código como el de Sensio y yo lo encuentro muy útil cuando se trabaja con el ORM de Doctrine. Esto me motivó a extender ese bundle y agregar las funcionalidades necesarias para trabajar con el _ODM_ de Doctrine, utilizando las herramientas que proporciona el proyecto mongodb-odm de Doctrine. Herramientas que permiten generar código para documentos y repositorios a partir de una instancia de [ClassMetadata][class-metadata](objeto que contiene información acerca del mapping de una entidad/documento).

_Puedes encontrar este bundle en su [**repositorio** en Github][repo]._

### Más información

En el archivo [README](https://github.com/iambrosi/IsmaAmbrosiGeneratorBundle/blob/master/README.md) se pueden encontrar más datos e instrucciones de instalación.


[class-metadata]: http://www.doctrine-project.org/api/common/2.2/class-Doctrine.Common.Persistence.Mapping.ClassMetadata.html "Doctrine\Common\Persistence\Mapping\ClassMetadata"


[repo]: https://github.com/iambrosi/IsmaAmbrosiGeneratorBundle "IsmaAmbrosiGeneratorBundle"
