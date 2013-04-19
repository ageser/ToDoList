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

Nat�rliche Person mit Name, Adresse usw.

Role
....

Rolle mit bestimmten Zust�ndigkeiten, F�higkeiten und Rechten in der Applikation.
Z.B. Teacher oder Student
Die einzelnen Rollen k�nnten als Traits implementiert und die F�higkeiten und Rechte darin ausprogrammiert werden.

User
....

Eine `Person`_, die sich in die Applikation einloggen und damit arbeiten kann.

Person - Role - User
....................

Eine Person kann mehrere Rollen einnehmen.
Z.B. kann ein Lehrer auch ein Sch�ler sein oder ein Schul-Administrator kann auch Lehrer sein.
Hat eine Person mehrere Rollen in denen er mit der Applikation arbeiten kann (z.B. Schul-Administrator und Lehrer), muss er sich beim Login entscheiden, in welcher der Rollen er arbeiten m�chte. Ein eingeloggter User ist also immer in genau einer Rolle und hat ausschliesslich die F�higkeiten und Rechte derselben.
