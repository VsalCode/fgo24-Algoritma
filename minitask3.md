## Menghitung Luas dan Keliling Lingkaran

#### Deskriptif :

1. Mulai
2. Masukkan nilai r (jari-jari)
3. jika r habis dibagi 7 , maka phi = 22/7
4. jika tidak, maka phi = 3,14
5. hitung Luas dengan phi x r  x r
5. hitung Keliling dengan 2 x phi x r
6. selesai

#### Flowchart menghitung luas

```mermaid
flowchart TD
    A@{shape: circle, label: "start"}
    B@{shape: lean-r, label: "input r"}
    C@{shape: diamond, label: "r % 7 == 0"}
    phi1@{shape: rect, label: "phi = 22/7"}
    phi2@{shape: rect, label: "phi = 3,14"}
    luas@{shape: rect, label: "Luas = phi x r x r"}
    keliling@{shape: rect, label: "Keliling = 2 x phi x r"}
    output@{shape: lean-r, label: "output: 'Keliling','Luas'"}
    X@{shape: dbl-circ, label: "stop"}

    A --> B
    B --> C
    C -- True --> phi1
    C -- False --> phi2
    
    phi1 --> luas
    phi1 --> keliling
    luas --> output 
    keliling --> output

    phi2 --> luas
    phi2 --> keliling
    luas --> output 
    keliling --> output
    
    output --> X

```

## Pseudo-code

```
DECLARE r: REAL
DECLARE Keliling: REAL
DECLARE Luas: REAL

INPUT r

IF r % 7 == 0 THEN
    Luas <- 22/7 x r x r  
    Keliling <- 2 x 22/7 x r    
ELSE
    Luas <- 3,14 x r x r  
    Keliling <- 2 x 3,14 x r
ENDIF

OUTPUT "K : ", Keliling, "L : ", Luas

```
