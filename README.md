# Latihan modul 10
Penjelasan singkat pada tiap latihan soal modul 7

## Setiap soal
Pada setiap soal saya menggunakan beberapa komponen :
- `Package main` agar program dapat dieksekusi
- `import fmt` agar dapat menggunakan beberapa operasi dasar bahasa program `go`
- `import math` agar dapat memasukkan fungsi matematika dalam program `go`
- `main()` sebagai titik awal program dan dieksekusi ketika program dijalankan

## Soal 1
```go
 minBerat := berat[0]
    maxBerat := berat[0]

    for i := 1; i < N; i++ {
        if berat[i] < minBerat {
            minBerat = berat[i]
        }
        if berat[i] > maxBerat {
            maxBerat = berat[i]
        }
    }
```
Operasi diatas merupakan operasi mencari dan menentukan nilai max dan nilai min pada suatu array

## Soal 2
```go
jumlahWadah := (x + y - 1) / y
var totalBerat []float64
for i := 0; i < jumlahWadah; i++ {
var sum float64
for j := i * y; j < min(i*y+y, x); j++ {
        sum += berat[j]
    }
    totalBerat = append(totalBerat, sum)
}
```
Operasi diatas merupakan operasi menghitung jumlah wadah yang dibutuhkan dengan pernyataan bahwa satu wadah memasukkan beberapa ikan kemudian menghitung total berat ikan pada setiap wadah

```go
var totalSemua float64
for _, beratWadah := range totalBerat {
        totalSemua += beratWadah
}
rataRata := totalSemua / float64(jumlahWadah)
```
Operasi diatas merupakan operasi menghitung rata-rata dari berat ikan pada setiap wadah

## Soal 3
```go
func hitungMinMax(arrBerat arrBalita, n int, bMin, bMax *float64) {
    *bMin = arrBerat[0]
    *bMax = arrBerat[0]

    for i := 1; i < n; i++ {
        if arrBerat[i] < *bMin {
            *bMin = arrBerat[i]
        }
        if arrBerat[i] > *bMax {
            *bMax = arrBerat[i]
        }
    }
}
```
Operasi diatas merupakan operasi mencari dan menentukan nilai max dan nilai min pada suatu array

```go
func rerata(arrBerat arrBalita, n int) float64 {
    total := 0.0
    for i := 0; i < n; i++ {
        total += arrBerat[i]
    }
    return total / float64(n)
}
```
Operasi diatas merupakan operasimenghitung rata rata dari total berat balita dengan jumlah balita yang ada pada array
