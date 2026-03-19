# [Construction d'une application Web à trois couches avec ASP.NET 2.0, C#, Spring.Net et NHibernate (2010)](https://stahe.github.io/pam-aspnet-juin-2010/)

Ce document présente la construction progressive de **SimuPaie**, une application .NET destinée à simuler le calcul de la paie d'assistantes maternelles. Le fil conducteur est double : **mettre en place une architecture logicielle claire** et **implémenter la solution avec les technologies .NET de l'époque**. Le support décrit en particulier une **architecture à trois couches** composée d'une couche d'accès aux données (DAO), d'une couche métier et d'une couche de présentation, le tout intégré par **Spring IoC**.

## Objectifs du cours

L'étude de cas a pour but de montrer comment concevoir une application Web maintenable en séparant clairement les responsabilités :

- **Couche 1 - DAO** : accès aux données stockées en base.
- **Couche 2 - Métier** : calculs de paie et règles fonctionnelles.
- **Couche 3 - UI** : interaction avec l'utilisateur et restitution des résultats.
- **Intégration** des couches par **interfaces .NET** et **injection de dépendances avec Spring IoC**.

Le document rappelle également le cycle de traitement d'une requête utilisateur : la demande est reçue par l'application, transmise si nécessaire à la couche métier puis à la couche d'accès aux données, avant qu'une réponse adaptée soit renvoyée au client.

## Versions successives de l'application

Le support ne se limite pas à une unique implémentation. Il propose plusieurs déclinaisons de SimuPaie afin d'illustrer différentes approches d'architecture et d'interface :

1. une version **ASP.NET mono-formulaire** en architecture une couche ;
2. une version équivalente enrichie avec **Ajax** ;
3. une version **ASP.NET en trois couches** avec **NHibernate** pour l'accès aux données ;
4. une version **multi-vues et mono-page** ;
5. une version orientée **service web** côté serveur ;
6. une version cliente ASP.NET consommant ce service ;
7. une version **multi-vues et multi-pages** ;
8. une version cliente du service web ;
9. une variante trois couches s'appuyant davantage sur des classes Spring facilitant l'usage de NHibernate ;
10. une version cliente **FLEX**.

## Prérequis

Le document s'adresse plutôt à un niveau **intermédiaire**. Il suppose des bases en :

- **ASP.NET**
- **C# 2008** : classes, interfaces, héritage, polymorphisme
- **Spring IoC / injection de dépendances**
- **architecture Web à trois couches** et modèle **MVC**.

## Outils et technologies abordés

L'étude de cas s'appuie sur un ensemble cohérent d'outils et de frameworks :

- **Visual C# 2008**
- **Visual Web Developer Express 2008**
- **SQL Server Express 2005**
- **Spring.Net / Spring IoC**
- **NHibernate**
- **NUnit** pour les tests unitaires.

## Ce que ce dépôt peut apporter

Ce support intéressera particulièrement les lecteurs qui veulent :

- comprendre la mise en oeuvre d'une **architecture n-tiers** en environnement .NET ;
- voir comment **découpler** la présentation, le métier et l'accès aux données ;
- découvrir l'usage de **Spring.Net** pour l'assemblage des composants ;
- étudier l'intégration de **NHibernate** dans une application Web ASP.NET ;
- suivre une progression pédagogique allant d'une version simple vers des versions plus industrialisées.

## Contenu du support

Le document expose l'architecture générale de l'application et illustre dès la première page, via un schéma, le rôle de l'utilisateur, de l'application, des trois couches et de Spring IoC dans l'orchestration de l'ensemble. Il sert donc à la fois de **cours d'architecture**, de **guide de conception** et de **base de travail pour une implémentation pratique**.

