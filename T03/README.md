# 🔐 Recuperació d’accés i fortificació del GRUB en Zorin OS

En aquesta tercera tasca, ens enfrontem a un problema habitual en entorns Linux: la pèrdua de la contrasenya d’usuari que impedeix l’accés a dades importants. El nostre client disposa d’un portàtil amb Zorin OS, un sistema Linux amb entorn gràfic, però no pot accedir-hi perquè ha oblidat la contrasenya. Per garantir la seguretat del sistema i evitar qualsevol risc de pèrdua o dany sobre l’equip original, treballarem sobre una còpia del disc original en una màquina virtual.

L’objectiu principal és recuperar l’accés al sistema modificant la contrasenya d’un usuari existent, tot aprofitant les vulnerabilitats del carregador d’arrencada GRUB. Posteriorment, i atenent a les preocupacions del client, investigarem com protegir l’accés al GRUB amb contrasenya per evitar que aquesta vulnerabilitat es pugui explotar en el futur.

---

## 🎯 Objectius de la pràctica

- Configurar una màquina virtual amb el disc clonat del portàtil.
- Identificar l’usuari existent al sistema Linux.
- Recuperar l’accés canviant la contrasenya de l’usuari.
- Investigar i implementar la protecció per contrasenya al GRUB.
- Documentar tot el procés, incloent-hi evidències gràfiques i fonts consultades.

---

Amb aquesta pràctica, aprofundirem en conceptes clau de la seguretat lògica a Linux, combinant l’explotació de vulnerabilitats amb mesures de protecció per reforçar la seguretat dels sistemes.
