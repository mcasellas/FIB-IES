# IES OCL (20-4-18)

### Especificació:

- Dades -> UML
- Operacions -> OCL

### Patrons típics:

#### Nova instància de classe:

|Pre|Post
-|-|-
Nova instància de classe | - | oclIsNew() + Atributs
Nova instància d'associaicó | Comprovar existència de l'extrem | Lligam
Nova instància de classe associativa | Comprovar existència de l'extrem | oclIsNew() + Atributs + Lligams
Especialització | Comprovar existència d'objecte | oclIsTypeOf()


`Exemple lligam:`
```java
p.recinte.nom -> includes(nomR)
``` 
