# Praktikum 5

## 5-1:
a) Failile on vaja 400, kaustale 100  
b) Failile on vaja 000, kaustale 300

## 5-2:
Skripti käivitamine nõuab lisaks käivitamisõigusele lugemisõigust.

## 5-3:
Iga kasutaja omanimeline grupp on kasulik lihtsustamaks faililubadega tegelemist.

## 5-4:
Vt. pilt  
<img width="960" alt="5-4-kassiga" src="https://github.com/karl-k-m/opsys/assets/74490726/d1a8f409-0448-4465-9c43-57e7f563bc64">

## 5-5:
vt. pilt  
<img width="960" alt="5-5-fix" src="https://github.com/karl-k-m/opsys/assets/74490726/a7ce10ec-e834-4290-b18e-10c55aaa6785">

## 5-6:
Juhul, kui see on valesti seadistatud, võib see anda failidele ligipääsu kasutajatele, kes seda ei tohiks saada.

## 5-7:
1. Faili omanik
2. Kausta omanik
3. root

## 5-8:
vt. pilt  
<img width="960" alt="5-8" src="https://github.com/karl-k-m/opsys/assets/74490726/ceb9ddd8-9d02-46fb-b387-f98b7ee3645c">

## 5-9
+i (immutable) tähendab, et faili ei saa modifitseerida ükski kasutaja, sh root. Et sellist faili kustutada, tuleb teha:  
sudo chattr -i fail.txt ;  
rm fail.txt
