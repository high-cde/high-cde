![high-cde — ZDOS Systems · Zlang Runtime · Automation Engineering](https://capsule-render.vercel.app/api?type=waving&color=0:0b1020,38:1d4ed8,70:7c3aed,100:10b981&height=220&section=header&text=high-cde&fontSize=68&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=ZDOS%20Systems%20%C2%B7%20Zlang%20Runtime%20%C2%B7%20Automation%20Engineering&descAlignY=60&descSize=18)

# Ciao, sono **high-cde**

[![ZDOS](https://img.shields.io/badge/ZDOS-x86__64%20prototype-2563eb?style=for-the-badge&logo=linux&logoColor=white)](https://github.com/high-cde/ZDOS/tree/main/os/x86_64)
[![Zlang](https://img.shields.io/badge/Zlang-ZLB0%20v1-7c3aed?style=for-the-badge&logo=rust&logoColor=white)](https://github.com/high-cde/Zlang)
[![QEMU](https://img.shields.io/badge/boot-QEMU%20verified-059669?style=for-the-badge&logo=qemu&logoColor=white)](https://github.com/high-cde/ZDOS/actions)
[![Automation](https://img.shields.io/badge/focus-automation%20%26%20systems-f59e0b?style=for-the-badge&logo=gnubash&logoColor=white)](https://github.com/high-cde?tab=repositories)

> **Costruisco sistemi modulari che si possano leggere, compilare e verificare.** Il focus attuale è trasformare l’ecosistema ZDOS in una catena tecnica concreta: da un programma Zlang, al bytecode, al kernel, fino a un’immagine avviabile in QEMU.

## ⚡ In evidenza: una pipeline che esiste davvero

![Pipeline Zlang → ZDOS](https://raw.githubusercontent.com/high-cde/ZDOS/main/os/x86_64/assets/zdos-zlang-pipeline.png)

| Passaggio | Cosa accade | Evidenza pubblica |
|---|---|---|
| 📝 **Zlang** | Un programma `emit <testo>` viene descritto in `.zlang` | [Compilatore ZLB0 v1](https://github.com/high-cde/Zlang/tree/main/tools) |
| ⚙️ **Bytecode** | `zlangc.py` genera un formato versionato e validabile | [Contratto tecnico](https://github.com/high-cde/Zlang/blob/main/docs/zdos-x86_64-profile.md) |
| 🧠 **Kernel** | Il bytecode viene incorporato ed eseguito dal kernel bare-metal | [ZDOS x86_64](https://github.com/high-cde/ZDOS/tree/main/os/x86_64) |
| 💿 **Boot** | GRUB crea l’ISO e QEMU verifica l’output seriale | [Workflow CI](https://github.com/high-cde/ZDOS/actions) |

> **Stato preciso:** si tratta di un prototipo x86_64 avviabile, non ancora di un sistema operativo generale. Processi, filesystem, rete, driver, loader esterno e syscall pubbliche sono tappe future, non promesse già realizzate.

## 🧭 Direzione tecnica

Il mio lavoro unisce progettazione, automazione e validazione. L’idea è semplice: prima un contratto piccolo e verificabile, poi una nuova capacità; mai il contrario.

| Pilastro | Obiettivo | Principio operativo |
|---|---|---|
| 🧠 **Sistemi intelligenti** | Orchestrazione, memoria e componenti modulari | Separare il comportamento dal contesto di esecuzione |
| ⚙️ **Automazione** | CLI, toolchain, wrapper e pipeline ripetibili | Un comando deve produrre un effetto osservabile |
| 🛡️ **Sicurezza difensiva** | Ambienti controllati, policy e test negativi | Default-deny, minimo privilegio, auditabilità |
| 💿 **ZDOS / Zlang** | Runtime nativo e sistema bare-metal incrementale | Sorgente → bytecode → kernel → boot → verifica |
| ☁️ **Web e Cloud** | Dashboard, integrazioni e servizi di supporto | Interfacce chiare, componenti riusabili, documentazione |

## 🧪 Progetti da esplorare

| Repository | Perché è importante |
|---|---|
| [**ZDOS**](https://github.com/high-cde/ZDOS) | Monorepo dell’ecosistema; include il prototipo bare-metal x86_64 avviabile in QEMU. |
| [**Zlang**](https://github.com/high-cde/Zlang) | Linguaggio applicativo e compilatore ZLB0 v1 usato dal prototipo ZDOS. |
| [**zdos-organism**](https://github.com/high-cde/zdos-organism) | Workspace sperimentale Rust/Python per runtime, VM e componenti osservabili. |
| [**ZCORE**](https://github.com/high-cde/ZCORE) | Esperimenti sul nucleo e sull’identità del sistema ZDOS. |
| [**Z-CYBERCORE**](https://github.com/high-cde/Z-CYBERCORE) | Ricerca e tooling per la sicurezza in contesti autorizzati e difensivi. |
| [**xCLOUD-by-zdos**](https://github.com/high-cde/xCLOUD-by-zdos) | Layer cloud e interfacce enterprise dell’ecosistema. |

## 🧩 Stack e strumenti

![Python](https://img.shields.io/badge/Python-14354C?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![Assembly](https://img.shields.io/badge/x86__64-Assembly-6E4C13?style=flat-square&logo=gnubash&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![QEMU](https://img.shields.io/badge/QEMU-FF6600?style=flat-square&logo=qemu&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

## 🎓 Metodo di lavoro

> **Progettare → implementare → testare → documentare → pubblicare.**

Ogni componente dovrebbe dichiarare con chiarezza ciò che funziona, ciò che rifiuta e ciò che è ancora in progetto. Per questo, nei repository ZDOS e Zlang, la documentazione non è un poster: è parte del contratto tecnico.

| Regola | Significato pratico |
|---|---|
| ✅ **Verificabile** | Build, test e output devono poter essere ripetuti da chiunque. |
| 🔒 **Esplicita** | Le capability di sistema devono essere ristrette e documentate. |
| 🧱 **Modulare** | Ogni livello ha responsabilità e confini definiti. |
| 📚 **Educativa** | Il percorso dal concetto alla macchina deve restare leggibile. |
| 🚀 **Incrementale** | Le promesse future seguono prove concrete, non le anticipano. |

## 📊 Attività GitHub

![Statistiche GitHub](https://github-readme-stats.vercel.app/api?username=high-cde&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github&locale=it)

![Linguaggi principali](https://github-readme-stats.vercel.app/api/top-langs/?username=high-cde&layout=compact&theme=tokyonight&hide_border=true&locale=it)

## 🤝 Contatti e collaborazioni

Se vuoi discutere architetture ZDOS, runtime, toolchain, automazione o sicurezza difensiva in ambienti autorizzati, puoi trovarmi qui:

| Canale | Riferimento |
|---|---|
| 📧 Email | [Highkali13@proton.me](mailto:Highkali13@proton.me) |
| 🌐 Web | [x-zdos.it](https://x-zdos.it) |
| 🐙 GitHub | [github.com/high-cde](https://github.com/high-cde) |

## 📚 Riferimenti

[1] [ZDOS — prototipo x86_64](https://github.com/high-cde/ZDOS/tree/main/os/x86_64)
[2] [Zlang — profilo ZLB0 v1](https://github.com/high-cde/Zlang/blob/main/docs/zdos-x86_64-profile.md)
[3] [Laboratorio ZDOS x86_64 + Zlang](https://github.com/high-cde/ZDOS/blob/main/os/x86_64/LEARNING_PATH.md)
[4] [Validazione continua ZDOS](https://github.com/high-cde/ZDOS/actions)
[5] [Validazione continua Zlang](https://github.com/high-cde/Zlang/actions)

---

**high-cde** · _Build what you can prove._ ✨

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:10b981,42:1d4ed8,100:7c3aed&height=120&section=footer)
