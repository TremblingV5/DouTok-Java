# DouTok-Interface

> A project for all code of protocol

## Module Structure

```
└─org
    └─doutok
        │  App.java
        │
        ├─body
        │  ├─request
        │  │  ├─comment
        │  │  ├─commentDomain
        │  │  ├─favorite
        │  │  ├─favoriteDomain
        │  │  ├─feed
        │  │  ├─message
        │  │  ├─messageDomain
        │  │  ├─publish
        │  │  ├─relation
        │  │  ├─relationDomain
        │  │  ├─user
        │  │  ├─userDomain
        │  │  └─videoDomain
        │  │
        │  └─response
        │      ├─comment
        │      ├─commentDomain
        │      ├─favorite
        │      ├─favoriteDomain
        │      ├─feed
        │      ├─message
        │      ├─messageDomain
        │      ├─publish
        │      ├─relation
        │      ├─relationDomain
        │      ├─user
        │      ├─userDomain
        │      └─videoDomain
        │
        ├─entity
        │      BaseResponse.java
        │      Comment.java
        │      FriendUser.java
        │      Message.java
        │      User.java
        │      Video.java
        │
        └─protocol
                CommentDomainService.java
                CommentService.java
                FavoriteDomainService.java
                FavoriteService.java
                FeedService.java
                MessageDomainService.java
                MessageService.java
                PublishService.java
                RelationDomainService.java
                RelationService.java
                UserDomainService.java
                UserService.java
                VideoDomainService.java

```
