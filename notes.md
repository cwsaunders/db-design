# Database design class 1 (sie 550-12, overall lecture 17):
https://www.youtube.com/watch?v=snerKYp3cuc
<br>
<b>Conceptual schema:</b><br>
- "What elements should the database contain?"
<br>
- Captures the essential data that needs to be stored and the relationship between entities
- Conceptual schema often first hand-drawn (sketched)
- Design process typically uses some basic conventions to formulate db
<br><br>
<b>First crack at conceptual schema design:</b>
<br>
- named entities (boxes)
- named relationships between entities (arrows)
<br><br>
<b>Entities:</b>
<br>
- entities are classes, not individuals
- A class is an abstraction for several individuals that all share common properties
<br><br>
<b>Entity-Relationship Diagrams (ER Diagrams)</b><br>
- Peter Chen
- classes as rectangles
- Relationships as diamonds linked to boxes
- attributes as ovals linked to boxes or relationships
- primarily a graphical language (with text as lables)
    - alphabet
    - syntax rules
- Appropriate for small mini-worlds
<br><br>
<b>3-Schema Architecture:</b><br>
- Conceptual/LogicalView (Objects, relationships) <-- database designer
- Internal/PhysicalView (Data structures (B+-trees,hash tables), files, records) <-- database implementer
- External/ApplicationView (Views, Interfaces) <-- users

<br>
<b>Logical schema vs conceptual schema:</b> while conceptual is diagrams (drawing boxes, etc.), logical is more into the actual code and<br>
written design of the database.
<br><br>

<b>DBMS:</b><BR>
- Data Definition Language (DDL) which is the logical model fed into the database
- Physical level:
    - storage in bits and bytes
    - refers to data in location on physical device
        - When items are removed and re-added they have new memory addresses
        - Often an operating system will go through a process called de-fragmentation. ( https://en.wikipedia.org/wiki/Defragmentation )
        - Sometimes addresses will even be on different devices
    - Physical level is especially concerned with performance, e.g. speed of retrieval.

<br>
<b>Designer's Perspective:</b><br>
- Conceptual (cognitive) --> logical --> physical<br>
- DB Admin perspective: physical --> logical