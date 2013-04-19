================
 Domain Analyse
================

:Autor: Benjamin Stalder
:Version: 0.1
:Status: Draft

.. contents:: Inhalt
   :depth: 4
.. section-numbering::
   :depth: 4

Einleitung
==========

Das ist das Domain Analyse Dokument.

Subdomains
==========

Subdomain Person
----------------

Klassendiagramm
^^^^^^^^^^^^^^^

.. image:: bilder/domain_diagram.png
   :width: 300px
   :align: center

Klassen Beschreibung
^^^^^^^^^^^^^^^^^^^^

Person
......

Natürliche Person mit Name, Adresse usw.

Role
....

Rolle mit bestimmten Zuständigkeiten, Fähigkeiten und Rechten in der Applikation.
Z.B. Teacher oder Student
Die einzelnen Rollen könnten als Traits implementiert und die Fähigkeiten und Rechte darin ausprogrammiert werden.

User
....

Eine `Person`_, die sich in die Applikation einloggen und damit arbeiten kann.

Person - Role - User
....................

Eine Person kann mehrere Rollen einnehmen.
Z.B. kann ein Lehrer auch ein Schüler sein oder ein Schul-Administrator kann auch Lehrer sein.
Hat eine Person mehrere Rollen in denen er mit der Applikation arbeiten kann (z.B. Schul-Administrator und Lehrer), muss er sich beim Login entscheiden, in welcher der Rollen er arbeiten möchte. Ein eingeloggter User ist also immer in genau einer Rolle und hat ausschliesslich die Fähigkeiten und Rechte derselben.
