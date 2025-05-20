# Tutorial 10

## Experiment 1.2: Understanding how it works

!(experiment 1.2)[./assets/experiment_1_2.png]

Dapat dilihat bahwa print yang terletak di paling bawah adalah print yang paling pertama muncul. Hal ini dikarenakan ketika melakukan spawner.spawn, program hanya akan menjadwalkan task tersebut, tetapi tidak secara langsung melakukannya. Task hanya akan dilakukan jika sudah dipanggil oleh executor.run() yang letaknya di bawah print terakhir. Oleh karena itu, kedua print yang di atas akan muncul setelah print yang terakhir muncul terlebih dahulu.
