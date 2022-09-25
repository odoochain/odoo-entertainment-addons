Artist
======
This module adds the concept of an ``Artist`` as an Odoo model.

.. contents:: Table of Contents

An artist is a general designation for an entity in the entertainment.
It can be a humorist, a stage band, an orchestra, a painter, etc.

The term artist does not represent a person.
It designates a group of people (members). It may however be composed of one person.

该模块将“艺术家”的概念添加为 Odoo 模型。

.. contents:: 目录

艺术家是娱乐界实体的总称。它可以是幽默家、舞台乐队、管弦乐队、画家等。艺术家一词并不代表一个人。它指定一组人（成员）。然而，它可以由一个人组成。

Context
-------
When designing the module, there was a choice to be made:

1. either a new kind of object for representing artist
2. or otherwise extend `res.partner`

One reason for seperating an artist in a separate model is the ambiguity between
the commercial entity that owns the artist and the artist itself.

Also there is a distinction between the contacts at the commercial entity
and the members of the artist.

在一个单独的模型中分离艺术家的一个原因是拥有艺术家的商业实体与艺术家本身之间的模糊性。
商业实体的联系人和艺术家的成员之间也有区别。

Artists
-------
The module defines the form view of an artist.

.. image:: static/description/artist_form.png

Partner
~~~~~~~
The field `Partner` of an artist designates the commercial entity (i.e. for invoicing purposes).

Members
~~~~~~~
An artist can have one or more members.

Members are contacts. Each of theme has a role.

.. image:: static/description/artist_member_list.png

Known Issues
~~~~~~~~~~~~
The module defines views for artists, roles and tags.
However, it does not add menu items for accessing these.
We encourage you to add the appropriate menu entries and access rights in a separate module depending on your use case.

Contributors
------------
* Numigi (tm) and all its contributors (https://bit.ly/numigiens)

More information
----------------
* Meet us at https://bit.ly/numigi-com
