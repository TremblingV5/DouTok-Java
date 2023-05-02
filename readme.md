# DouTok-Java

> Java version of [DouTok](https://github.com/TremblingV5/DouTok)

[TOC]

## Child Projects Structure

### Public Projects

- DouTok-Interface
  > A project for all code of protocol
- DouTok-Common
  > A project contains some tools and secondary packaging

### Projects of Logic Layer

- DouTok-Api
- DouTok-Comment
- DouTok-Favorite
- DouTok-Feed
- DouTok-Message
- DouTok-Publish
- DouTok-Relation
- DouTok-User

### Projects of Domain Layer

- DouTok-CommentDomain
- DouTok-FavoriteDomain
- DouTok-MessageDomain
- DouTok-RelationDomain
- DouTok-UserDomain
- DouTok-VideoDomain

## Directory Structure of Child Projects

> Base on DDD

- api
  > Layer of user interface
  - controller
    > Layer of controller, implements of api of a non-distributed application 
  - dto
    > Layer of DTO (Data Transform Object), although it will be inplemented in `DouTok-Interface`
  - handler
    > Layer of handler, implements of api of a distributed application
  - misc
    > Miscellaneous of `api` layer, implements some logics like parameters checking
- application
  > Layer of applications
  - XXXManager.java
    > For finishing some logics rely on other layers
  - XXXEventProcessor.java
- domain
  > Layer of domain
  - enums
  - event
    > Implement some Java class for XXX event, like using it on MQ
  - impl
    > Implements of service, api of `domain`, for XXXManager to call
  - model
    > Data model
  - repository
    > Declare interfaces for db logics
  - service
    > Declare interfaces for all layer
- infrastructure
  > Layer of db, mq, cache, remote interfaces, search engine, third party tools and infrastructures
  - cache
  - client
  - dao
  - impl
    > Implements of `domain.repository`
  - mq
