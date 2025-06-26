# 📊 Analisi Statistica di un Testo

Questo progetto implementa un algoritmo che analizza un testo e restituisce alcune statistiche linguistiche fondamentali.  
L’analisi avviene attraverso l’elaborazione formale del testo e si basa su criteri linguistici e computazionali ben definiti.

---

## 🎯 Obiettivo del Programma

Dato un testo in input (stringa arbitraria), l’algoritmo:

- Estrae tutte le parole, ignorando punteggiatura e simboli speciali
- Calcola il numero **totale** di parole (con ripetizioni)
- Determina il numero di **parole uniche** (distinte, case-insensitive)
- Calcola la **frequenza** di ogni parola
- Identifica la **parola più lunga**

---

## ⚙️ Caratteristiche del Trattamento Testuale

- Le **lettere accentate** (à, è, ì, ò, ù) sono considerate parte dell’alfabeto e vengono mantenute.
- La distinzione tra maiuscole e minuscole viene **annullata** (case-insensitive).
- I simboli di punteggiatura e i caratteri speciali sono **ignorati**.
- Le parole sono definite come **sequenze massimali** di lettere contigue.
- L’output finale è una struttura ordinata e leggibile delle statistiche del testo.

---

## 📌 Output Atteso

Il programma deve stampare i seguenti dati:

1. Numero totale di parole
2. Numero di parole uniche
3. Frequenza di ogni parola (in formato `parola → occorrenze`)
4. La parola più lunga presente nel testo

---

## 💡 Esempio di Esecuzione dell’Algoritmo

### 📝 Testo di Input
“Ciao! Mi chiamo Andrea. Ciao, ciao...”

### 🔹 Passo 1 – Pulizia del testo

Sostituzione dei caratteri non alfabetici con spazi:
"Ciao Mi chiamo Andrea Ciao ciao "

---

### 🔹 Passo 2 – Separazione in parole

Separazione per spazi, con rimozione delle stringhe vuote:

```json
["Ciao", "Mi", "chiamo", "Andrea", "Ciao", "ciao"] 
```
### 🔹 Passo 3 – Normalizzazione
```json
["ciao", "mi", "chiamo", "andrea", "ciao", "ciao"]
```

### 🔹 Passo 4 – Output
Numero totale di parole: 6  
Numero di parole uniche: 4

Frequenze:
- ciao → 3
- mi → 1
- chiamo → 1
- andrea → 1

Parola più lunga: chiamo
