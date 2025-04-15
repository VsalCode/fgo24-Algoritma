## Algoritma Konversi Suhu 

#### Deklaratif

1. mulai
1. masukkan suhu sebagai "c"
1. masukkan tipe konversi yang dipilih sebagai "type"
1. jika "type" = f, maka konversi menjadi "result = (9/5) × °C + 32"
1. jika "type" = k, maka konversi menjadi "result = °C + 273,15"
1. jika "type" = r, maka konversi menjadi "result = (4/5) × °C"
1. jika tidak, maka akhiri
1. selesai

#### Flowchart pemilihan type

```mermaid
flowchart TD
    A@{shape: circle, label: "start"}
    input@{shape: lean-r, label: "input: c"}
    type@{shape: lean-r, label: "input: type"}
    selector1{"type === 'f'"} 
    selector2{"type === 'k'"} 
    selector3{"type === 'R'"}
    result1@{shape: rectangle, label: "result = (9/5) × °C + 32"}
    result2@{shape: rectangle, label: "result = °C + 273,15"}
    result3@{shape: rectangle, label: "result = (4/5) × °C"}
    output@{shape: lean-r, label: "result"}
    X@{shape: dbl-circ, label: "end"}

    A --> input
    input --> type
    type --> selector1
    selector1 -- FALSE--> selector2
    selector1 -- TRUE --> result1
    result1 --> output


    selector2 -- FALSE --> selector3
    selector2 -- TRUE --> result2
    result2 --> output
    
    output --> X
    selector3 -- FALSE --> X
    selector3 -- TRUE --> result3
    result3 --> output

    

```


### Notes