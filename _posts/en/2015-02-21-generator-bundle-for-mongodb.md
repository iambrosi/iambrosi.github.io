---
layout: post
title:  Generator bundle for MongoDB
description: Introducing a generator bundle for MongoDB documents
name: IsmaAmbrosiGeneratorBundle
categories: [symfony, bundle]
tags: ['introduction']
---

[_IsmaAmbrosiGeneratorBundle_][repo] is an extension of the bundle [SensioGeneratorBundle](https://github.com/sensiolabs/SensioGeneratorBundle) for [Symfony](http://symfony.com) applications that allows to generate _documents_, _forms_ and _CRUD_ controllers to manage those MongoDB documents.

_The bundle **SensioGeneratorBundle** is included by default in the standard edition of the Symfony framework. You can find more information at the [official documentation](http://symfony.com/doc/master/bundles/SensioGeneratorBundle/index.html) page._

It provides interactive commands that let you generate code, with some help of the Doctrine's [mongodb-odm](https://github.com/doctrine/mongodb-odm) library.

I started working on this bundle a few years ago, but I don't know why, I never made an official announcement. I should have done it a long time ago.

It all started when I was working at ServerGrove, and MongoDB was the main database engine... and it was great. Symonfy2 was just showing up, its stable version hadn't been released yet, but it worked great for us.

The problem was that didn't exist a code generator like Sensio's, and for me it's very useful when you work with Doctrine's ORM. This pushed me to extend that bundle and include the necessary features to make it work with Doctrine's ODM, using the tools provided by the project mongodb-odm by Doctrine. Tools that allow to generate code for documents and repositories from an instance of [ClassMetadata][class-metadata] (object that contains mapping information about an entity/document).

_You can find this bundle in its own [**repository** on Github][repo]._

### More info

You can find some more information and installation instructions in the [README](https://github.com/iambrosi/IsmaAmbrosiGeneratorBundle/blob/master/README.md) file. And of course, everyone is welcome to participate and collaborate.


[class-metadata]: http://www.doctrine-project.org/api/common/2.2/class-Doctrine.Common.Persistence.Mapping.ClassMetadata.html "Doctrine\Common\Persistence\Mapping\ClassMetadata"


[repo]: https://github.com/iambrosi/IsmaAmbrosiGeneratorBundle "IsmaAmbrosiGeneratorBundle"
