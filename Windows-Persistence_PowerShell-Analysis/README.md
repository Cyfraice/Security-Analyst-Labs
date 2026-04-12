# Scenario 06: Windows Persistence & PowerShell Analysis


**Tipo:** Case study / Analisi forense  
**Autore:** Francesco Golisciano  
**Data:** 22/12/2023

---

### Obiettivi
Analisi di una macchina Windows compromessa per identificare meccanismi di persistenza e script offuscati.

### Tool utilizzati
* **Analisi Host:** `schtasks.exe`, `tasklist`, `PowerShell`
* **Network Forensics:** `tshark`, `Wireshark`

### Highlights dell'analisi
1. **Identificazione Persistenza:** Scoperta di 3 task schedulati malevoli (`task1`, `task2`, `task3`).
2. **De-offuscamento PowerShell:** - Analisi di payload in **Base64**.
   - Decodifica di stringhe offuscate tramite **XOR** (byte 33 e 30).
   - Identificazione della tecnica di chiamata dinamica a `IEX` tramite slicing di variabili d'ambiente.
3. **Analisi Traffico:** Correlazione tra esecuzione dei task e download di payload HTTP esterni.
