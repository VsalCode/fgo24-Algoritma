## Membuat algoritma ganjil dan genap

1. mulai
2. masukkan angka
3. jika angka tersebut habis dibagi dua, angka genap
4. jika tidak, angka ganjil 
5. selesai

## Flowchart ganjil genap

#### Flowchart :

```mermaid
flowchart TD
    A@{shape: circle, label: "start"}
    B@{shape: lean-r, label: "input r"}
    C@{ shape: diamond, label: "X % 2 = 0" }
    D@{shape: lean-r, label: " 'Genap' "}
    E@{shape: lean-r, label: " 'Ganjil' "}
    X@{shape: dbl-circ, label: "stop"}

    A --> B
    B --> C
    C -- True --> D
    C -- False --> E

    D --> X
    E --> X

```
