# IES - Introducció a la Enginyeria del Software:

> Teoria: Raimon Lapuente
>
> Laboratori: Xavier Oriol

----
## Problemes 1:
**Exemple datàfon pagament:**

Casos d'ús a l'UML: `Descripció d'un servei com una seqüencia d'esdeveniments.`
> Passar targeta per pagar -> Comprovar saldo...

Escenari d'un cas d'ús: `Sequència d'accions i d'interaccios entre els actors i el sistema.`
> En cas d'error, entitat d'una altra entitat...

Actors d'un cas d'ús: `Entitat externa que participa`
> Persones, organitzacions, hardware...

----
## Problemes 2:

> Si vull tenir atribut `nul`: crèdits: Real [0..1]

Assignatura|
-|
codi: String |
mon: String |
crèdits: Real |
tipus: TipusAssig |

<< enumeration >> *TipusAssig*|
-|
- obligatori |
- opcional |

> [0..1] Estableix claus primàries.

**Restriccions textuals:**

`- Claus externes:`
(Assignatura, codi)
(Assignatura, nom)
(Aula, codi)
(Dia i Hora, dia + hora)
(NumGrup, num)

~`- Una assignatura no pot ser prerequisit d'ella mateixa`~ (IES-> BD; BD-> IES) `- L'associació TéPrerequisits és acíclica.`

`- Una assignatura no pot ser corequisit d'ella mateixa.`

`- Si A té com a corequisit B, llavors B té com a corequisit A.`
> No té sentit que una assignatura en tingui i la relacionada no.

`- Clau dèbil:` No hi ha 2 grups d'assignatura amb el mateix número i assignatura.
