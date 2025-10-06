

# Informe SAI Everpia

**Nombre:** [Pol Castaño Meneses]  
**Fecha:** [06/10/2025]

<img src="img/Logo.png" alt="Logo" width="200">
---
# **ÍNDEX**

- [**1. Introducció**](#1-introducció)
- [**2. Inventari d’equips**](#2-inventari-dequips)
- [**2.1. Especificacions tècniques**](#21-especificacions-tècniques)
- [**3. Càlcul de potència total**](#3-càlcul-de-potència-total)
- [**4. Autonomia Requerida**](#4-autonomia-requerida)
- [**5. Recerca de models de SAI**](#5-recerca-de-models-de-sai)

---

# 1. **Introducció**

L’empresa **TecnoGestió S.L.**, especialitzada en gestió documental i assessorament informàtic, disposa d’un petit despatx amb quatre ordinadors de sobretaula, una impressora-fotocopiadora multifunció i un router d’accés a Internet.

A causa de les constants incidències en el subministrament elèctric a la zona, la direcció ha pres la decisió d’adquirir un **Sistema d’Alimentació Ininterrompuda (SAI)** amb l’objectiu de garantir la continuïtat del servei, protegir els equips informàtics i assegurar la integritat de les dades.

Aquest informe té com a finalitat **analitzar les necessitats energètiques del despatx, calcular la potència requerida, determinar l’autonomia mínima necessària i presentar diferents opcions de SAI** disponibles al mercat, amb la finalitat de recomanar la solució més adequada segons els requeriments de l’empresa.

# 2. **Inventari d’equips**

| Dispositiu | Quantitat | Connectar al SAI? | Justificació |
| :---- | :---- | :---- | :---- |
| Ordinadors de Sobretaula | 4 | Sí |  |
| Monitors | 4 | Sí |  |
| Impressora Mulifunció | 1 | No | No es posaria, ja que no és un aparell essencial pel funcionament de l'empresa |
| Router | 1 | Sí |  |

# 2.1 **Especificacions tècniques**

**Ordinadors de Sobretaula: [Ryzen](https://www.pccomponentes.com/pc-racing-ofimatica-amd-ryzen-3200g-8gb-480gb-ssd-windows-11)**

* **Model estimat**: PC racing  
* **Placa Base:** B450  
* **Processador**: AMD Ryzen 3 3200G  
* **RAM**: 8GB DDR4  
* **Emmagatzematge**: 512GB SSD M.2 Nvme  
* **Font d’alimentació**: 500W  
* **Consum:** 300w  
* **Consum Real:** 333,33VA

**Monitors:**

* **Model:** Monitor MSI PRO MP225 21.5" LED IPS FullHD 100Hz  
* **Tassa de refresc:** 100 Hz  
* **Mida:** 21.5"  
* **Consum:** 15w  
* **Consum Real:** 16,67VA

**Router:** 

* **Consum:** 5W  
* **Consum Real:** 5,56VA

# 3. **Càlcul de potència total** 

| Dispositiu | Quantitat | Consum en VA |
| ----- | :---: | :---: |
| Ordinadors | 4 | 1332 VA |
| Monitors | 4 | 66,68 VA |
| Router | 1 | 5,56 VA |
|  | SUMA TOTAL: | 1404,24 VA |
|  | \+20% RESERVA | 1686 VA |

Després del càlcul, ens ha resultat una quantitat total de **1.404,24 VA**. Hi afegim un **20 %** de reserva per garantir un funcionament estable i evitar sobrecàrregues, de manera que la potència requerida pel SAI és de **1.686 VA.**

# 4. **Autonomia Requerida** 

Tenint en compte els requeriments de l’empresa, guardar de manera segura els documents en curs i apagar correctament els ordinadors, es considera que un **temps d’autonomia acceptable i estàndard és d’entre 10 i 15 minuts**.

Aquest marge permet als usuaris finalitzar les tasques, desar els treballs oberts i efectuar un tancament ordenat dels equips sense risc de pèrdua de dades ni danys als sistemes.

Per tant, **aquest estudi ha establert com a valor mínim recomanat una autonomia de 10 minuts**.  
Tanmateix, **si es vol disposar de més flexibilitat**, és recomanable que el SAI ofereixi una autonomia aproximada de **20 minuts**, la qual cosa permetria mantenir el servei actiu durant interrupcions breus o repeticions de talls de subministrament elèctric.

Addicionalment, cal tenir present que:

* L’autonomia real pot variar segons la **càrrega connectada** i l’**estat de la bateria**.

* Els valors d’autonomia declarats pels fabricants són **orientatius** i poden disminuir amb el pas del temps o amb condicions ambientals adverses.

10\*1686/0,9/60 \= 312,222AH

La capacitat de la bateria perquè duri uns 10 minuts hauria de ser de 312.2AH.

# 5. **Recerca de models de SAI** 

Després d’una recerca dels diferents SAI dins de les especificacions requerides pel client, s’ofereixen tres opcions:

1. Bàsica: una solució econòmica que cobreix els requeriments mínims.

2. Intermèdia: un model amb més potència i funcionalitats, dins d’un rang mitjà.

3. Premium / completa: un SAI amb més potència i capacitat, per si cal connectar més equips en el futur o garantir més autonomia i marge de seguretat.

| SAI | SPS 2000 ONE | SPS 2200 SOHO+ | SPS 2000 ADV T |
| :---- | :---- | :---- | :---- |
| Potencia (VA/W) | 2000 VA / 1200 W | 2200 VA / 1200 W | 2000 VA / 1400 W |
| Autonomia | Fins a 20 minuts (Càrrega Baixa) | Fins a 18 minuts (Càrrega Alta) | Fins a 15 minuts (Càrrega mitjana) |
| Tipus de Sortides | 4 Schuko, port USB, protecció telèfon/ADSL | 4 Schuko o IEC, 2 USB frontals, LCD | 6 IEC C13, USB \+ RS232 \+ ranura SNMP, LCD |
| Preu € | 176,04 € (Amazon) | 235,99 € (PcComponentes) | 354,32 € (Amazon) |

Per a les necessitats actuals de l’empresa, **el model més adequat és el SPS 2000 ONE**, ja que:

* Ofereix prou potència i autonomia mínima requerida.  
* És l'opció més econòmica i pràctica per a una petita oficina.  
* Permet assegurar el correcte apagament i protecció dels equips sense necessitat de gastar en funcions avançades que no s’utilitzaran immediatament.

Si l’empresa preveu **ampliar els equips o necessitar un control més avançat**, es podria considerar el **SPS 2000 ADV T**, tot i que suposa un cost superior i ofereix més funcions de les que el despatx actual necessita.

---

[Tornar al Enunciat](README.md) 
