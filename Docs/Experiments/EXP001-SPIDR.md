# EXP001 - SPIDR

## Finding

F002

## Observation

AI langsung memilih satu pola SPIDR tanpa mengevaluasi alternatif.

## Hypothesis

Jika prompt meminta AI membandingkan minimal dua alternatif SPIDR sebelum memilih satu, maka reasoning SPIDR akan menjadi lebih baik.

## Prompt Change

Instruksi SPIDR diubah agar AI:

- membandingkan minimal dua alternatif,
- menjelaskan kelebihan,
- menjelaskan kekurangan,
- menjelaskan alasan memilih satu pola.

## Test Case

TC01

## Result

Berhasil.

AI mengevaluasi dua pola SPIDR (Simple/Complex dan Rules), menjelaskan trade-off masing-masing, kemudian memberikan alasan mengapa Simple/Complex dipilih.

## Conclusion

Hipotesis didukung.

Perubahan layak dimasukkan ke Prompt V2.
