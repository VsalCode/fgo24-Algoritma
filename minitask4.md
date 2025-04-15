## mengubah algoritma celcius 

#### Deklaratif

1. mulai
2. deklarasikan bahwa 0 derajat celcius = 32 fahrenheit
3. deklarasikan bahwa 0 derajat celcius = 273 kelvin
4. masukkan nilai suhu dalam bentuk celcius
4. masukkan nilai suhu dalam bentuk celcius


#### Flowchart

```mermaid
flowchart TD
    A@{shape: circle, label: "start"}
    B@{shape: lean-r, label: "input suhu(celcius)"}
    C@{ shape: diamond, label: "pilih opsi konversi" }
    D@{ shape: rect, label: "0 C = 32 fahrenheit" } 
    E@{ shape: rect, label: "0 C = 273 kelvin" } 
    F@{ shape: rect, label: "0 C = 273 kelvin" } 
    G@{ shape: lean-r, label: "output suhu konversi" } 
    X@{shape: dbl-circ, label: "stop"}

    A --> B
    B --> C
    C --> D
    C --> E
    C --> F
    D --> G
    E --> G
    F --> G
    G --> X

```


