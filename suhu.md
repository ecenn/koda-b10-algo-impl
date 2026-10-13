# Konversi Suhu

Data input dimasukkan dalam satuan Celcius dan data output memberikan 3 nilai untuk satuan Farenheit, Kelvin, dan Reamur.

## Deskriptif

1. Mulai
2. Masukkan nilai Celcius (c)
3. Menghitung nilai Farenheit (f) dengan mengalikan nilai c dengan 9 dibagi dengan 5 lalu ditambah 32
4. Menghitung nilai Reamur (r) dengan mengalikan nilai c dengan 4 lalu dibagi 5
5. Menghitung nilai Kelvin (k) dengan menambahkan nilai c dengan 273
6. Menampilkan nilai f, r dan k
7. Selesai

## Flowchart

```mermaid

flowchart LR

a((start))
b[/c/]
c[f = c * 9 / 5 + 32]
d[r = c * 4 / 5]
e[k = c + 273]
f[/f/]
g[/r/]
h[/k/]
z(((stop)))

a --> b --> c --> d --> e --> f --> g --> h --> z

```

## Pseudocode

    DECLARE c : REAL
    DECLARE f : REAL
    DECLARE r : REAL
    DECLARE k : REAL
    INPUT c

    f <- c * 9 / 5 + 32
    r <- c * 4 / 5
    k <- c + 273

    OUTPUT f, r, k