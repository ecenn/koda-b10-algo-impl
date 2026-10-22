# Materi: Implementasi Algoritma

## Program: Kecepatan Lari

### Deskriptif
1. Mulai
2. Masukkan jarak lari (dalam km)
3. Masukkan waktu lari (dalam menit)
4. Hitung kecepatan lari (pace) dengan membagi waktu lari dengan jarak lari
5. Apabila hanya ingin lihat pace saja, maka tampilkan pace
6. Hitung kecepatan lari di treadmill (speed) dengan membagi 60 dengan pace
7. Tampilkan pace dan speed
6. Selesai

### Flowchart

```mermaid

flowchart LR

a((start))
b[/jarak/]
c[/waktu/]
d[pace = waktu / jarak]
e{lihatPaceSaja?}
f[speed = 60 / pace]
g[/speed/]
h[/pace/]
z(((stop)))

a --> b --> c --> d --> e
e --true--> h
e --false--> f
f --> g
g --> h
h --> z

```

### Pseudocode

    DECLARE jarak : REAL            // satuan km
    DECLARE waktu : REAL            // satuan min
    DECLARE pace : REAL             // satuan min/km
    DECLARE speed : REAL            // satuan km/jam
    DECLARE lihatPaceSaja : BOOLEAN
    INPUT jarak
    INPUT waktu
    INPUT lihatSpeed

    pace <- waktu / jarak

    IF lihatPaceSaja = TRUE THEN
        OUTPUT pace
    ELSE
        speed <- 60 / pace
        OUTPUT speed, pace
    ENDIF
