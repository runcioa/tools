# gobuster

## Semplice guida all'uso
  
Uno dei primi step nell'attaccare un'applicazione web è quella di riuscire a vedere le directory e i file nascosti.

### Vantaggi

Gobuster rispetto ad altri (DirBuster e DIRB) essendo implementato in Go risulta essere più veloce.

### Svantaggi

Risulta più lento rispetto altri altri nel caso in cui si debbano fare ricerche ricorsive cioè i percorsi annidati anche solo di un livello.

---

#### Uso normale

Per effettuare una scansione della macchina si utilizza un file già presente in kali linux presente nella directory `/usr/share/wordlists`:

`gobuster -u http://<IP macchina>/<directory>/ -w /usr/share/wordlists/common.txt`

La scansione ritorna il nome delle directory, dei file e l'HTTP response code.

```bash

---


#### Fonti

* [Markdown-Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#html) Guida per scrtivere questo documento