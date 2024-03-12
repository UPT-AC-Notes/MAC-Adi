- Urmărim folosirea a câtor mai puține operații de adunare și înmulțire în calculul polinoamelor
$$P\left( x\right) =2x^{4}+3x^{3}-3x^{2}+5x-1$$
- Metoda 1
$$p\left( \dfrac{1}{2}\right) =2\times \dfrac{1}{2}\times \dfrac{1}{2}\times \dfrac{1}{2}\times \dfrac{1}{2}+3\times \dfrac{1}{2}\times \dfrac{1}{2}\times \dfrac{1}{2}-3\times \dfrac{1}{2}\times \dfrac{1}{2}+5\times \dfrac{1}{2}-1=1.25$$
- nr de înmulțiri necesare = 10
- nr de adunări necesare = 4

- Metoda 2
	- putem ține minte calculul fiecărei puteri și să ne folosim mai apoi de acest rezultat pentru a calcula puteri de ordin mai mare
	- acest lucru duce la:
	- nr. de înmulțiri = 7
	- nr. de adunări = 4

- Metoda 3 (înmulțarea imbricată)
$$\begin{aligned}P\left( x\right) =-1+x\left( 5-3x+3x^{2}+2x^{3}\right) ,\\
P\left( x\right) =-1+x\left( 5+x\left( -3+3x+2x^{2}\right) \right) ,\\
P\left( x\right) =-1+x\left( 5+x\left( -3+x\left( 3+2x\right) \right) \right) ,\end{aligned}$$
- Evaluând expresia dinspre interior spre exterior, avem nevoie de:
- 4 înmulțiri
- 4 adunări

## Conversie baza 10-baza 2
- Fie n = 53,7 în B 10
- luăm reparat 53 și 0,7
- 53 în B1O = 11 0101 în B 2
- partea fracționară:(înmulțim cu baza)
$$\begin{aligned}0,7\times 2\rightarrow 0,4+1,\\
0,4\times 2\rightarrow 0,8+0,\\
0,8\times 2\rightarrow 0,6+1,\\
0,6\times 2\rightarrow 0,2+1,\\
0,2\times 2\rightarrow 0,4+0,\\
0,4\times 2\rightarrow 0,8+0\\
\vdots \end{aligned}$$
- Observăm că acest proces se va repeta la infinit după cel de-al cincelea pas, cu perioada pe ultimii 4 pași⇒ 0,7 în B10 este 0,1 (0110) in B 2
- Concluzionăm că 53,7 în B10 este 110101, 1 (0 110) în B2

## Conversie baza 2- baza 10
- Pentru parte întreagă adunăm baza ridicată la puterea greutății doar dacă bitul este 1, ex:
$$110101=2^{5}+2^{4}+2^{2}+2^{0}=53$$
- Dacă partea fracționară este finită procedăm în aceeași manieră
$$0,1011=2^{-1}+2^{-3}+2^{-4}=\dfrac{1}{2}+\dfrac{1}{8}+\dfrac{1}{16}=\dfrac{11}{16}$$
- Dificultatea apare în calculul părții fracționare care nu este finită
	- cea mai simplă metodă de convertire a unei secvențe binare periodice într-o fracție Zecimală este de a folosi proprietatea de deplasare a înmulțirii cu 2 (Baza)
$$\begin{aligned}x=0,\left( 1011\right) ,\\
2^{4}\times x=1011,\left( 1011\right) ,\\
\Rightarrow x\left( 2^{4}-1\right) =\left( 1011\right) _{2}=\left( 11\right) _{10},\\
\Rightarrow x=0,\left( 1011)\right) _{2}=\left( \dfrac{11}{15}\right) _{10}\end{aligned}$$
- Dacă avem un număr care conține și o parte fracționară fixă și una periodică, înmulțim cu 2 până ajungem să avem doar parte fracționară periodică
$$\begin{aligned}x=\left( 0,10\left( 101\right) \right) _{2},\\
y=2^{2}x=10,\left( 101\right) \Rightarrow Z=0,\left( 101\right) \Rightarrow 2^{3}Z=101,\left( 101\right) \Rightarrow \ldots \end{aligned}$$

## Conversie baza 2- baza 16

- Separăm numărul binar în grupuri de câte 4, deoarece 2 la puterea 4 este 16, apoi fiecare grupă se va transforma într-un singur caracter din baza 16