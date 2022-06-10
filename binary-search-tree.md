# [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

İkili arama ağacı, her düğümün solundaki koldan ulaşılabilecek bütün verilerin düğümün değerinden küçük, sağ kolundan ulaşılabilecek verilerin değerinin o düğümün değerinden büyük olmasını şart koşar.

| Açıklama 	|  	|  	|  	|
|---	|---	|---	|---	|
| Root =7 	|  	| 7 	|  	|

5 sayısı 7'den küçük olduğunda 7'nin soluna ekledik

| Açıklama 	|  	|  	|  	|
|---	|---	|---	|---	|
|  	|  	|  	| 7 	|
|  	|  	| / 	|  	|
|  5 Ekledik	| 5 	|  	|  	|

1 sayısı 5'ten ve 7'den küçük olduğunda 7 ve 5'in soluna ekledik

| Açıklama 	|  	|  	|  	|  	|  	|
|---	|---	|---	|---	|---	|---	|
|  	|  	|  	|  	|  	| 7 	|
|  	|  	|  	|  	| / 	|  	|
|  	|  	|  	| 5 	|  	|  	|
|  	|  	|/  	|  	|  	|  	|
| 1 ekledik 	| 1 	|  	|  	|  	|  	|

8 sayısı 7'den büyük olduğunda 7'nin sağına ekledik

| Açıklama 	|  	|  	|  	|  	|  	|
|---	|---	|---	|---	|---	|---	|
|  	|  	|  	|  7	|  	|  	|
|  	|  	| / 	|  	|  	|  	|
|  	| 5 	|  	|  	| / 	|  	|
|  	|  /	|  	|  	|  	| 8 	|
| 1 	|  	|  	|  	|  	|  	|
|  	|  \	|  	|  	|  	|  	|
|  	|  	| 3 	|  	|  	|  	|

3 sayısı 7'den ve 5'ten küçük olduğunda 5'in soluna, 1'den büyük olduğunda 1'in sağına ekledik

| Açıklama 	|  	|  	|  	|  	|  	|  	|  	|
|---	|---	|---	|---	|---	|---	|---	|---	|
|  	|  	|  	|  	|  	| 7 	|  	|  	|
|  	|  	|  	|  	| / 	| \ 	|  	|  	|
|  	|  	|  	|  5	|  	|  	|  	| 8 	|
|  	|  	|/  	|  	|  	|  	|  	|  	|
|  	| 1 	|  	|  	|  	|  	|  	|  	|
|  	|  	| \ 	|  	|  	|  	|  	|  	|
| 3 ekledik 	|  	|  	| 3 	|  	|  	|  	|  	|

2 sayısı 7'den ve 5'ten küçük olduğunda 5'in soluna, 1'den büyük olduğunda 1'in sağına ve 3'ten küçük olduğunda 3'ün soluna ekledik

| Açıklama 	|  	|  	|  	|  	|  	|  	|  	|  	|  	|  	|  	|
|---	|---	|---	|---	|---	|---	|---	|---	|---	|---	|---	|---	|
|  	|  	|  	|  	|  	|  	|  	|  7	|  	|  	|  	|  	|
|  	|  	|  	|  	|  	|  	| / 	|  	|\  	|  	|  	|  	|
|  	|  	|  	|  	|  	|  5	|  	|  	|  	| 8 	|  	|  	|
|  	|  	|  	|  	| / 	|  	|  \	|  	|  	|  	|  	|  \	|
|  	|  	|  	| 1 	|  	|  	|  	| 6 	|  	|  	|  	|  	9|
|  	|  	|  /	|  \	|  	|  	|  	|  	|  	|  	|  	|  	|
|  	| 0 	|  	|  	|  3	|  	|  	|  	|  	|  	|  	|  	|
|  	|  	|  	|  	|  	|  	|\  	|  	|  	|  	|  	|  	|
|  	|  	|  	|  	|  	|  	|  	| 4 	|  	|  	|  	|  	|