## Menghitung Luas dan Keliling Lingkaran

#### Deskriptif :

1. Mulai
2. Masukkan nilai r (jari-jari)
3. jika r habis dibagi 7 maka, phi = 22/7
4. jika tidak, maka phi = 3,14
5. hitung luas lingkaran dengan phi x r  x r
5. hitung keliling lingkaran dengan 2 x phi x r
6. selesai

#### Flowchart menghitung luas

```mermaid
flowchart TD
    A@{shape: circle, label: "start"}
    B@{shape: lean-r, label: "input r"}
    C@{shape: diamond, label: "r % 7 == 0"}
    D@{shape: rect, label: "phi = 22/7"}
    E@{shape: rect, label: "phi = 3,14"}
    F@{shape: rect, label: "phi x r x r"}
    X@{shape: dbl-circ, label: "stop"}

    A --> B
    B --> C
    C -- True --> D
    C -- False --> E
    D --> F
    E --> F
    F --> X

```

#### Flowchart menghitung keliling

```mermaid
flowchart TD
    A@{shape: circle, label: "start"}
    B@{shape: lean-r, label: "input r"}
    C@{shape: diamond, label: "r % 7 == 0"}
    D@{shape: rect, label: "phi = 22/7"}
    E@{shape: rect, label: "phi = 3,14"}
    F@{shape: rect, label: "2 x phi x r"}
    X@{shape: dbl-circ, label: "stop"}

    A --> B
    B --> C
    C -- True --> D
    C -- False --> E
    D --> F
    E --> F
    F --> X

```

## Pseudo-code

#### Menghitung Luas
```
DECLARE r: REAL
DECLARE Result: REAL

INPUT r

IF r % 7 = 0 THEN
    Result <- 22/7 x r x r  
ELSE
    Result <- 3,14 x r x r  
ENDIF

OUTPUT Result

```

#### Menghitung Keliling
```
DECLARE r: REAL
DECLARE Result: REAL

INPUT r

IF r % 7 = 0 THEN
    Result <- 2 x 22/7 x r  
ELSE
    Result <- 2 x 2,14 x r  
ENDIF

OUTPUT Result

```
