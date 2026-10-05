# PEUnSN
Viola Jones Face Detection on system level abstraction

KRATKO POJASNJENJE PROGRAMA
Uslov:
-jedini prihvatljiv RGB format .jpg
-slika MORA biti sacuvana kao input.jpg

RUN:
make
./facedetect.exe

CLEANUP:
make clean

1.Pokretanje :
make
./facedetect.exe

2.Ciscenje objektnih datoteka:
make clean

3.Funkcionalnosti fajlova:

input.jpg: slika nad kojom se vrsi implementacija detekcije lica
Makefile: kompajlerski fajl
parameter.txt: sadrzi vrijednosti shiftStep i scaleFactor parametara potrebnih za izgradnju piramide slika kod detekcije lica

.cpp i .h fajlovi :

define: definicije konstanti i drugih globalnih promjenljivih
facedetect : implementacija rada detektora lica 
image : operacije nad greyscale slikom
image_ops : preprocessing operacije za RGB sliku
stb biblioteke : biblioteke za rad sa JPG formatom.
tb_facedetect : testbench detektora lica

.dat fajlovi - sadrze klasifikacione parametre za detekciju lica, konkretno :

rectangles: Geometrijske podatke Haarovih karakteristika;
stages: Strukturu klasifikacione kaskade (faze klasifikacije);
weights: Tezinu (vaznost) individualnih karakteristika;
alpha1 i alpha2: Koeficijente slabih klasifikatora (pozitivnih i negativnih);
tree_thresh: Pragove klasifikacije svih slabih klasifikatora;
stages_thresh: Pragove klasifikacije svake faze klasifikacije;
