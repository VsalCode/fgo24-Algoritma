## Membuat algoritma ganjil dan genap

1. mulai
2. masukkan angka sebagai "X"
3. jika "X" tersebut habis dibagi dua, "X" adalah Angka Genap
4. jika tidak, "X" Adalah Angka Ganjil 
5. selesai

## Flowchart ganjil genap

#### Flowchart :

```mermaid
flowchart TD
    A@{shape: circle, label: "start"}
    B@{shape: lean-r, label: "`X`"}
    C@{ shape: diamond, label: "X % 2 == 0" }
    D@{shape: lean-r, label: " 'Angka Genap' "}
    E@{shape: lean-r, label: " 'Angka Ganjil' "}
    X@{shape: dbl-circ, label: "end"}

    A --> B
    B --> C
    C -- True --> D
    C -- False --> E

    D --> X
    E --> X

```
## Pseudo-code

```
DECLARE X: INTEGER
DECLARE Result: STRING

INPUT X

IF X % 2 == 0 THEN
    Result <- " adalah angka Genap"
ELSE
    Result <- " adalah angka Ganjil"
ENDIF

OUTPUT X, Result
```
