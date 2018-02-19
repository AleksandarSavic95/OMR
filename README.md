# OMR
Me and my brother's attempt of OMR (Optical Music Recognition) implementation in Python, using OpenCV. In the beginning, we will try to read monophonic photos of printed data. After that, we will try our luck and knowledge in polyphonic pieces (such as piano sheets) and monophonic hand-writings. 

This project was chosen as part of the "Soft computing" course on the fourth year of "Software engineering and information technology" studies.

Faculty of technical sciences, Novi Sad, school year 2017/2018.

[Link to the issue on the course's github repository](https://github.com/ftn-ai-lab/sc-2017-siit/issues/15)

::: POKRETANJE PROJEKTA :::
===
1 - Pokretanje okruženja
===
Prvi način
---
1) Preuzeti i raspakovati .zip fajl repozitorijuma
2) U **komandnoj liniji** pozicionirati se u folder projekta (OMR)
3) Pokrenuti Jupyter Notebook aplikaciju iz komandne linije naredbom  *jupyter notebook*

Drugi način - pravljenjem batch (.bat) fajla sa sljedećim sadržajem:
---
    @echo off
    DRIVE:
    cd\PUTANJA_DO_FOLDERA_PROJEKTA
    start .
    jupyter notebook

DRIVE --> ime particije (npr. "c" ili "d", *bez* navodnika)

2 - Upotreba
===
1) Fotografija koju treba obraditi mora biti u folderu projekta, ili nekom od njegovih podfoldera, radi pristupa iz jupyter nootebook-a,
2) U promjenljivu `IMAGE_PATH` upisati putanju do te fotografije,
3) Kliknuti na prvu ćeliju projekta i iz menija *Cell* odabrati *Run all*

### Rezultat izvršavanja
U folderu sa putanje iz promjenljive `RESULTS_PATH` (postavljena vrijednost je *'./results'*) nalaziće se:
 - **XML datoteka** sa generisanim MusicXML sadržajem
 - **fotografija sa uklonjenim notnim linijama**, čiji naziv sadrži naziv ulazne fotografije, kao i parametre sa kojima je obrađivana

U istom folderu nalaziće se fotografije koje su nastale tokom obrade:
 - `dil_1_50.jpg`,
 - `er_2_50_dil_1_50.jpg`
