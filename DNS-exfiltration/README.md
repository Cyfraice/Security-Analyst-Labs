# Case Study - Analisi di un'esfiltrazione dati via DNS

**Tipo:** Case study / Analisi forense  
**Autore:** Francesco Golisciano  
**Data:** 4/12/2023

---

## Sommario
Analisi tecnica di un'esfiltrazione simulata di un file tramite interrogazioni DNS di tipo TXT. Il documento descrive i passaggi di analisi host e network, le evidenze raccolte, la ricostruzione del file e le raccomandazioni operative per contenimento e detection.

> **Nota importante:** questo report è una mia rielaborazione personale di uno scenario simulato affrontato in un percorso formativo organizzato da Fastweb Digital Academy in collaborazione con docenti universitari. Tutti i dati sensibili (IP, nomi utenti, host, screenshot) sono stati anonimizzati per la pubblicazione. Gli indirizzi compaiono come IP-vittima e IP-attaccante.

---

## Contenuto del repository

/case-study-dns-exfiltration/
├── Golisciano_case-study_dns-exfiltration.pdf # Report (anonimizzato)
├── README.md


---

## Abstract tecnico
Un processo sulla macchina vittima si riattiva ogni trenta secondi e invia porzioni di un file dentro interrogazioni DNS di tipo TXT, verso un server DNS controllato dall'attaccante. I nomi di host del dominio `akvz.com` contengono il file codificato in Base64. L'analisi ha incluso: enumerazione dei processi, esame del file system e della storia del repository, cattura e analisi PCAP, decodifica e ricostruzione del file, e mappatura su MITRE ATT&CK (T1059.004, T1071.004, T1048.003, T1027).

---

## Competenze dimostrate
- **Host forensics:** analisi processi, file system, storia del repository.  
- **Network forensics:** cattura e analisi PCAP (tshark/Wireshark), identificazione del traffico DNS TXT.  
- **Analisi del meccanismo:** decodifica Base64 dei nomi di host e ricostruzione del file.  
- **Threat modeling:** mappatura delle tecniche su MITRE ATT&CK.  
- **DevSecOps:** raccomandazioni operative (contenimento, logging DNS, resolver autorizzati, baseline su /opt, SIEM).

---

## Come consultare il materiale
1. Scarica il repository.  
2. Apri `Golisciano_case-study_dns-exfiltration.pdf` per il documento completo e narrativo.  

> **Nota di sicurezza:** il report è una rielaborazione didattica. Non contiene credenziali valide né dati reali non anonimizzati.

---

## Se vuoi contattarmi
- **LinkedIn:** [(link al profilo) ](https://it.linkedin.com/in/francesco-golisciano-ba436a126) 

---

## Licenza e uso
Questo materiale è pubblicato a scopo dimostrativo e didattico per il mio portfolio personale. Se intendi riutilizzare parti significative, cita la fonte e contattami per autorizzazione.

---

**Versione breve per descrizione pubblicazioni:**  
Case study tecnico: analisi forense di un'esfiltrazione dati via DNS - analisi host e network, ricostruzione del file, mappatura MITRE e raccomandazioni DevSecOps.
