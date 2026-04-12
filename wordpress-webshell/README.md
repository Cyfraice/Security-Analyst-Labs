# Case Study – Analisi di un attacco WordPress tramite Web Shell

**Tipo:** Case study / Analisi forense  
**Autore:** Francesco Golisciano  
**Data:** 22/12/2023

---

## Sommario
Analisi tecnica di una compromissione simulata di un'istanza WordPress tramite web shell PHP distribuite in più directory. Il documento descrive i passaggi di analisi host e network, le evidenze raccolte, la ricostruzione del payload e le raccomandazioni operative per remediation e detection.

> **Nota importante:** questo report è una mia rielaborazione personale di uno scenario simulato affrontato in un percorso formativo organizzato da Fastweb Digital Academy in collaborazione con docenti universitari. Tutti i dati sensibili (IP, nomi utenti, host, screenshot) sono stati anonimizzati per la pubblicazione.

---

## Contenuto del repository

/case-study-wordpress-webshell/
├── Golisciano_scenario5.pdf # Report (anonimizzato)
├── README.md


---

## Abstract tecnico
Un attaccante ha ottenuto esecuzione di comandi su un’istanza WordPress attraverso web shell (es. `backdoor.php`, `revshell.php`, file 404 alterato). Sono state osservate esecuzioni via HTTP, reverse shell verso un endpoint esterno e scrittura di output su file `.pwned.txt`. L’analisi ha incluso: enumerazione processi, confronto hash dei file malevoli, cattura e analisi PCAP, estrazione e ricostruzione del payload, e mappatura su MITRE ATT&CK.

---

## Competenze dimostrate
- **Host forensics:** analisi processi, file system, verifica hash.  
- **Network forensics:** cattura e analisi PCAP (tshark/Wireshark), identificazione reverse shell.  
- **Malware analysis:** analisi di web shell PHP e tecniche di offuscamento.  
- **Threat modeling:** mappatura tattiche su MITRE ATT&CK.  
- **DevSecOps:** raccomandazioni operative (re-image, rotazione credenziali, SAST/SCA, WAF, SIEM).

---

## Come consultare il materiale
1. Scarica il repository.  
2. Apri `report.pdf` per il documento completo e narrativo.  

> **Nota di sicurezza:** il report è una rielaborazione didattica. Non contiene credenziali valide né dati reali non anonimizzati.

---

## Se vuoi contattarmi
- **LinkedIn:** [(link al profilo) ](https://it.linkedin.com/in/francesco-golisciano-ba436a126) 

---

## Licenza e uso
Questo materiale è pubblicato a scopo dimostrativo e didattico per il mio portfolio personale. Se intendi riutilizzare parti significative, cita la fonte e contattami per autorizzazione.

---

**Versione breve per descrizione pubblicazioni:**  
Case study tecnico: analisi forense di compromissione WordPress via web shell — analisi host & network, ricostruzione payload, mappatura MITRE e raccomandazioni DevSecOps.
