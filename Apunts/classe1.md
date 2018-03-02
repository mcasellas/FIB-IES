# IES - Introducció a la Enginyeria del Software:

> Teoria: Raimon Lapuente
>
> Laboratori: Xavier Oriol

----
## Laboratori 1:
**Exemple datàfon pagament**

Casos d'ús a l'UML: `Descripció d'un servei com una seqüencia d'esdeveniments.`
> Passar targeta per pagar -> Comprovar saldo...

Escenari d'un cas d'ús: `Sequència d'accions i d'interaccios entre els actors i el sistema.`
> En cas d'error, entitat d'una altra entitat...

Actors d'un cas d'ús: `Entitat externa que participa`
> Persones, organitzacions, hardware...

----
## Laboratori 2:

> Si vull tenir atribut `nul`: crèdits: Real [0..1]

Assignatura|
-|
codi: String |
mon: String |
crèdits: Real |
tipus: TipusAssig |

<< enumeration >> TipusAssig|
-|
- obligatori |
- opcional |


**Restriccions textual:**

`- Claus externes:`
(Assignatura, codi)
(Assignatura, nom)
(Departament, nom)

~`- Una assignatura no pot ser prerequisit d'ella mateixa`~ `- L'associació *TéPrerequisits* és acíclica`
