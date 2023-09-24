%Appunti Teorici di Matematica
%Federico Zotti
%18/12/2022

# Funzioni

## Funzioni reali di variabile reale

Dati due sottoinsiemi A e B (non vuoti) di $\mathbb{R}$, una funzione $f$ da A a B è una relazione che associa a ogni numero reale di A _uno e un solo_ numero reale di B.

$$
f: A \rightarrow B
$$

## Dominio naturale (campo di esistenza)

Il dominio naturale della funzione $y=f(x)$ è l'insieme più ampio dei valori reali che si possono assegnare alla variabile indipendente $x$ affinché esista un corrispondente valore reale $y$.

## Proprietà delle funzioni

Una funzione da A a B è:

- **Iniettiva** se ogni elemento di B è immagine di al più un elemento di A;

- **Suriettiva** se ogni elemento di B è immagine di almeno un elemento di A;

- **Biunivoca** se è sia iniettiva che suriettiva.

## Funzione crescente

- $y=f(x)$ di dominio $D \subseteq \mathbb{R}$ è una funzione **crescente** se in un intervallo $I \subseteq D$ se scelti $x_1, x_2$ $\in I$ con $x_1 < x_2$ risulta $f(x_1) \leq f(x_2)$.

- $y=f(x)$ di dominio $D \subseteq \mathbb{R}$ è una funzione **strettamente crescente** se in un intervallo $I \subseteq D$ se scelti $x_1, x_2$ $\in I$ con $x_1 < x_2$ risulta $f(x_1) < f(x_2)$.

## Funzione decrescente

- $y=f(x)$ di dominio $D \subseteq \mathbb{R}$ è una funzione **crescente** se in un intervallo $I \subseteq D$ se scelti $x_1, x_2$ $\in I$ con $x_1 < x_2$ risulta $f(x_1) \geq f(x_2)$.

- $y=f(x)$ di dominio $D \subseteq \mathbb{R}$ è una funzione **strettamente crescente** se in un intervallo $I \subseteq D$ se scelti $x_1, x_2$ $\in I$ con $x_1 < x_2$ risulta $f(x_1) > f(x_2)$.

## Funzione peridodica

$y = f(x)$ è una funzione **periodica** di periodo $T$, con $T > 0$ se per qualsiasi numero $k$ intero si ha:
$$
f(x) = f(x + kT)
$$

## Funzione pari

$D \subseteq \mathbb{R}$ tale che, se $x \in D$, allora $-x \in D$.

$y = f(x)$ è una funzione **pari** in $D$ se $\forall x \in D$:
$$
f(-x) = f(x)
$$

## Funzione dispari

$D \subseteq \mathbb{R}$ tale che, se $x \in D$, allora $-x \in D$.

$y = f(x)$ è una funzione **dispari** in $D$ se $\forall x \in D$:
$$
f(-x) = -f(x)
$$

# Limiti

## Intorno di un punto

Dato un numero reale $x_0$, un **intorno completo** di $x_0$ è un qualunque intervallo aperto $I(x_0)$ contenente $x_0$ ($\delta_1$ e $\delta_2$ numeri reali positivi):
$$
I(x_0) = ] x_0 - \delta_1 ; x_0 + \delta_2 [
$$

## Intorno circolare

Dato un numero reale $x_0$ e un numero reale positivo $\delta$, un **intorno circolare** di $x_0$, di raggio $\delta$ è l'intervallo aperto $I_\delta(x_0)$ di centro $x_0$ e raggio $\delta$:
$$
I_\delta(x_0) = ] x_0 - \delta ; x_0 + \delta [
$$

## Punto di accumulazione

Il numero reale $x_0$ è un **punto di accumulazione** di $A \subseteq \mathbb{R}$ se ogni intorno completo di $x_0$ contiene infiniti punti di $A$.

## $\boldsymbol{ \lim_{x \to x_0 }f(x)=\ell }$

La funzione $f(x)$ ha per limite il numero reale $\ell$, per $x$ che tende a $x_0$, quando, comunque si scelga un numero reale positivo $\epsilon$, si può determinare un intorno completo $I(x_0)$ tale che:
$$
\forall \epsilon > 0 \exists I(x_0):
$$
$$
| f(x) - \ell | < \epsilon,
$$
$$
\forall x \in I(x_0), x \neq x_0
$$

## Funzione continua

Siano $f(x)$ una funzione definita in un intervallo $[a;b]$ e $x_0$ un punto interno all'intervallo.
La funzione $f(x)$ è **continua nel punto $x_0$** quando esiste il limite di $f(x)$ per $x \to x_0$ e tale limite è uguale al valore $f(x_0)$ della funzione calcolata in $x_0$:
$$
\forall x_0 \in [a;b] \rightarrow \lim_{x \to x_0} f(x) = f(x_0)
$$

## Limite per eccesso

Diciamo che $f(x)$ tende a $\ell$ **per eccesso** e scriviamo:
$$
\lim_{x \to x_0} f(x) = \ell^+
$$
se $f(x)$ è una funzione con limite finito $\ell$ per $x$ che tende a $x_0$ e assume sempre valori _maggiori_ di $\ell$ in un intorno di $x_0$ con al più $x \neq x_0$.

## Limite per difetto

Diciamo che $f(x)$ tende a $\ell$ **per difetto** e scriviamo:
$$
\lim_{x \to x_0} f(x) = \ell^-
$$
se $f(x)$ è una funzione con limite finito $\ell$ per $x$ che tende a $x_0$ e assume sempre valori _minori_ di $\ell$ in un intorno di $x_0$ con al più $x \neq x_0$.

## $\boldsymbol{ \lim_{x \to x_0 }f(x)= + \infty }$

Se $f(x)$ una funzione definita in un intervallo $[a;b]$ e non definita in $x_0 \in [a;b]$.
$f(x)$ tende a $+\infty$ per $x$ che tende a $x_0$ quando per ogni numero reale positivo $M$ si può determinare un intorno completo $I(x_0)$ tale che:
$$
\forall M > 0 \exists I(x_0):
$$
$$
f(x) > M,
$$
$$
\forall x \in I(x_0), x \neq x_0
$$

## $\boldsymbol{ \lim_{x \to x_0 }f(x)= - \infty }$

Se $f(x)$ una funzione definita in un intervallo $[a;b]$ e non definita in $x_0 \in [a;b]$.
$f(x)$ tende a $-\infty$ per $x$ che tende a $x_0$ quando per ogni numero reale positivo $M$ si può determinare un intorno completo $I(x_0)$ tale che:
$$
\forall M > 0 \exists I(x_0):
$$
$$
f(x) < -M,
$$
$$
\forall x \in I(x_0), x \neq x_0
$$

## Asintoto verticale

Data la funzione $y=f(x)$, se si verifica che:
$$
\lim_{x \to c} f(x) = \pm \infty
$$
la retta $x=c$ è **asintoto verticale** per il grafico della funzione.

## $\boldsymbol{ \lim_{x \to + \infty }f(x)= \ell}$

Una funzione $f(x)$, definita in un intervallo illimitato a destra, tende al numero reale $\ell$ per $x$ che tende a $+\infty$ quando, per ogni $\epsilon > 0$ fissato, si può determinare un intorno $I$ di $+\infty$ tale che:
$$
\forall \epsilon > 0 \exists c > 0:
$$
$$
| f(x) - \ell | < \epsilon,
$$
$$
\forall x > c
$$

## $\boldsymbol{ \lim_{x \to - \infty }f(x)= \ell}$

Una funzione $f(x)$, definita in un intervallo illimitato a destra, tende al numero reale $\ell$ per $x$ che tende a $-\infty$ quando, per ogni $\epsilon > 0$ fissato, si può determinare un intorno $I$ di $-\infty$ tale che:
$$
\forall \epsilon > 0 \exists c > 0:
$$
$$
| f(x) - \ell | < \epsilon,
$$
$$
\forall x < -c
$$

## Asintoto orizzontale

Data la funzione $y=f(x)$, se si verifica una delle condizioni:
$$
\lim_{x \to +\infty} f(x) = q \qquad \lim_{x \to -\infty} f(x) = q \qquad \lim_{x \to \infty} f(x) = q
$$
la retta $y=q$ è **asintoto orizzontale** per il grafico della funzione.

## $\boldsymbol{ \lim_{x \to \pm \infty }f(x)= \pm \infty}$

### $\boldsymbol{ \lim_{x \to +\infty }f(x)= +\infty}$

Una funzione $f(x)$, definita in un intervallo illimitato a destra, ha per limite $+\infty$ per $x$ che tende a $+\infty$ quando, per ogni numero reale positivo $M$, si può determinare un intorno $I$ di $+\infty$ tale che:
$$
\forall M > 0 \exists c > 0:
$$
$$
f(x) > M,
$$
$$
\forall x > c
$$

### $\boldsymbol{ \lim_{x \to -\infty }f(x)= +\infty}$

Una funzione $f(x)$, definita in un intervallo illimitato a sinistra, ha per limite $+\infty$ per $x$ che tende a $-\infty$ quando, per ogni numero reale positivo $M$, si può determinare un intorno $I$ di $-\infty$ tale che:
$$
\forall M > 0 \exists c > 0:
$$
$$
f(x) > M,
$$
$$
\forall x < -c
$$

### $\boldsymbol{ \lim_{x \to +\infty }f(x)= -\infty}$

Una funzione $f(x)$, definita in un intervallo illimitato a destra, ha per limite $-\infty$ per $x$ che tende a $+\infty$ quando, per ogni numero reale positivo $M$, si può determinare un intorno $I$ di $+\infty$ tale che:
$$
\forall M > 0 \exists c > 0:
$$
$$
f(x) < -M,
$$
$$
\forall x > c
$$

### $\boldsymbol{ \lim_{x \to -\infty }f(x)= -\infty}$

Una funzione $f(x)$, definita in un intervallo illimitato a sinistra, ha per limite $-\infty$ per $x$ che tende a $-\infty$ quando, per ogni numero reale positivo $M$, si può determinare un intorno $I$ di $-\infty$ tale che:
$$
\forall M > 0 \exists c > 0:
$$
$$
f(x) < -M,
$$
$$
\forall x < -c
$$

## Teorema di unicità del limite

Se per $x \to x_0$ la funzione $f(x)$ ha per limite il numero reale $\ell$ allora tale limite è unico.

## Teorema della permanenza del segno

Se il limite di una funzione per $x \to x_0$ è un numero $\ell$ diverso da 0, allora esiste un intorno $I(x_0)$ (escluso al più $x_0$) in cui $f(x)$ e $\ell$ sono entrambi positivi oppure entrambi negativi.

## Teorema del confronto

Siano $h(x), f(x), g(x)$ tre funzioni definite in uno stesso intorno $H$ di $x_0$, escluso al più il punto $x_0$.
Se in ogni punto di $H$ diverso da $x_0$ risulta:
$$
h(x) \leq f(x) \leq g(x)
$$
e il limite delle due funzioni $h(x)$ e $g(x)$, per $x \to x_0$, è uno stesso numero $\ell$, allora anche $\lim_{x \to x_0} f(x) = \ell$.

$$
\left.
	\begin{aligned}
		& h(x) \leq f(x) \leq g(x) \\
		& \lim_{x \to x_0} h(x) = \ell \\
		& \lim_{x \to x_0} g(x) = \ell
	\end{aligned}
\right\} \rightarrow \lim_{x \to x_0} f(x) = \ell
$$

## Funzione continua

Una funzione definita in $[a;b]$ si dice **continua** nell'intervallo $[a;b]$ se è continua in ogni punto dell'intervallo.

## Teorema di Weierstrass

se $f$ è una funzione continua in un intervallo limitato e chiuso $[a;b]$, allora essa assume, in tale intervallo, il massimo assoluto e il minimo assoluto.

## Teorema dei valori intermedi

Se $f$ è una funzione continua in un intervallo limitato e chiuso $[a;b]$, allora essa assume, almeno una volta, tutti i valori compresi tra il massimo e il minimo.

## Teorema di esistenza degli zeri

Se $f$ è una funzione continua in un intervallo limitato e chiuso $[a;b]$ e negli estremi di tale intervallo assume valori di segno opposto, allora esiste almeno un punto $c$, interno all'intervallo, in cui $f$ si annulla, ossia $f(c) = 0$.

## Punti di discontinuità

### Prima specie

Un punto $x_0$ si dice **punto di discontinuità di prima specie** per la funzione $f(x)$ quando, per $x \to x_0$, il limite destro e il limite sinistro di $f(x)$ sono entrambi finiti ma diversi fra loro:
$$
\lim_{x \to x_0^-} f(x) = \ell_1 \neq \lim_{x \to x_0^+} f(x) = \ell_2
$$

La differenza $|\ell_2 - \ell_1|$ si dice **salto** della funzione.

### Seconda specie

Un punto $x_0$ si dice **punto di discontinuità di seconda specie** per la funzione $f(x)$ quando per $x \to x_0$ almeno uno dei due limiti, destro o sinistro, di $f(x)$ è infinito oppure non esiste.

### Terza specie

Un punto $x_0$ si dice **punto di discontinuità di terza specie** per la funzione $f(x)$ quando:
$$
\lim_{x \to x_0} f(x) \neq f(x_0)
$$

## Asintoto obliquo

La retta di equazione $y = mx+q$ con $m \neq 0$ è **asintoto obliquo** di una funzione $f(x)$ se:
$$
\lim_{x \to x_0} [ f(x) - (mx+q)] = 0
$$

Per trovarlo:
$$
m = \lim_{x \to x_0} \frac{f(x)}{x}
$$
$$
q = \lim_{x \to x_0} [f(x) - mx]
$$

# Derivate

## Rapporto incrementale

Dati una funzione $y = f(x)$, definita in un intervallo $[a;b]$, e due numeri reali $c$ e $c+h$ (con $h \neq 0$) interni all'intervallo, il **rapporto incrementale** di $f$ nel punto $c$ (o relativo a $c$) è il numero:
$$
\frac{\Delta y}{\Delta x} = \frac{f(c+h)-f(c)}{h}
$$

## Derivata di una funzione

Dati una funzione $y = f(x)$, definita in un intervallo $[a;b]$, la **derivata della funzione** nel punto $c$ interno all'intervallo, che indichiamo con $f'(c)$, è il limite, se esiste ed è _finito_ per $h \to 0$, del rapporto incrementale di $f$ relativo a $c$:
$$
f'(c) = \lim_{h \to 0} \frac{f(c+h)-f(c)}{h}
$$

La derivata di $f$ nel punto $c$ è il coefficiente angolare della retta tangente in $c$.

Una funzione è derivabile in un intervallo chiuso $[a;b]$ se è derivabile in tutti i punti interni dell'intervallo e se esistono e sono finite la derivata destra in $a$ e la derivata sinistra in $b$.

Se una funzione è derivabile nel punto $x_0$, inquel punto la funzione è anche continua.

## Retta tangente

Data la funzione $y=f(x)$, l'equazione della retta tangente al grafico di $f$ nel punto $(x_0;y_0)$, se tale retta esiste e non è parallela all'asse $y$, è:
$$
y - y_0 = f'(x_0) \cdot (x-x_0)
$$

## Punto stazionario

Dati la funzione $y=f(x)$ e un suo punto $x=c$, se $f'(c) = 0$, allora $x=c$ è un **punto stazionario** o un **punto a tangente orizzontale**.

## Criterio di derivabilità

Se $f(x)$ è una funzione continua in $[a;b]$, derivabile in $]a;b[$ tranne al più in $x_0 \in ]a;b[$ e se:
$$
\lim_{x \to x_0^-} f'(x) = \lim_{x \to x_0^+} f'(x) = \ell
$$
allora la funzione è derivabile in $x_0$ e risulta:
$$
f'(x) = \ell
$$

## Differenziale di una funzione

Il **differenziale** di una funzione $f(x)$, relativo al punto $x$ e all'incremento $\Delta x$, è il prodotto della derivata della funzione, calcolata in $x$, per l'incremento $\Delta x$.
Il differenziale viene indicato con $\mathrm{d} f(x)$ oppure $\mathrm{d} y$:
$$
\mathrm{d}y = f'(x) \cdot \Delta x
$$

## Teorema di Lagrange

Se una funzione  $f(x)$ è continua in un intervallo chiuso $[a;b]$ ed è derivabile in ogni punto interno a esso, esiste almeno un punto $c$ interno ad $[a;b]$ per cui vale la relazione:
$$
\frac{f(b)-f(a)}{b-a} = f'(c)
$$

### Conseguenze

Se una funzione $f(x)$ è continua nell'intervallo $[a;b]$, derivabile in $]a;b[$ e tale che $f'(x)$ è nulla in ogni punto interno dell'intervallo, allora $f(x)$ è costante in tutto $[a;b]$.

Se $f(x)$ e $g(x)$ sono due funzioni continue nell'intervallo $[a;b]$, derivabili in $]a;b[$ e tali che $f'(x) = g'(x) \ \forall x \in ]a;b[$, allora esse differiscono per una costante.

## Teorema di Rolle

Se, per una funzione $f(x)$ continua nell'intervallo $[a;b]$ e derivabile nei punti interni di questo intervallo, si ha la condizione $f(a) = f(b)$, allora esiste almeno un punto $c$, interno all'intervallo, per il quale risulta:
$$
f'(c) = 0
$$

## Teorema di Cauchy

Se le funzioni $f(x)$ e $g(x)$ sono continue nell'intervallo $[a;b]$, derivabili in ogni punto interno a questo intervallo e inoltre in $]a;b[$ è sempre $g'(x) \neq 0$, allora esiste almeno un punto $c$ interno ad $[a;b]$ in cui si ha:
$$
\frac{f(b)-f(a)}{g(b)-g(a)} = \frac{f'(c)}{g'(c)}
$$
cioè il rapporto fra gli incrementi delle funzioni $f(x)$ e $g(x)$ nell'intervallo è uguale al rapporto fra le rispettive derivate calcolate in un particolare punto $c$ all'interno dell'intervallo.

## Teorema di De L'Hospital

Dati un intorno $I$ di un punto $c$ e due funzioni $f(x)$ e $g(x)$ definite in $I$ (escluso al più $c$), se:

- $f(x)$ e $g(x)$ sono derivabili in $I$ (escluso al più $c$), con $g'(x) \neq 0$;

- le due funzioni tendono entrambe a $0$ o a $\pm \infty$ per $x \to c$;

- per $x \to c$ esiste il limite del rapporto $\frac{f'(x)}{g'(x)}$;

allora esiste anche il limite del rapporto delle funzioni ed è:
$$
\lim_{x \to c} \frac{f(x)}{g(x)} = \lim_{x \to c} \frac{f'(x)}{g'(x)}
$$

## Massimo

### Assoluto

Data una funzione $y = f(x)$ il cui dominio è $D$, $x_0$ è il **punto di massimo assoluto** se:
$$
f(x) \leq f(x_0) \forall x \in D
$$

Il valore $f(x_0) = M$ è il **massimo assoluto** della funzione.

### Relativo

Data una funzione $y = f(x)$, definita in un intervallo $[a;b]$, $x_0$ è un **punto di massimo relativo** se esiste un intorno $I$ di $x_0$ tale che:
$$
f(x_0) \geq f(x) \forall x \in I(x_0)
$$

Il valore $f(x_0)$ è detto **massimo relativo** della funzione in $[a;b]$.

## Minimo

### Assoluto

Data una funzione $y = f(x)$ il cui dominio è $D$, $x_0$ è il **punto di minimo assoluto** se:
$$
f(x) \geq f(x_0) \forall x \in D
$$

Il valore $f(x_0) = M$ è il **minimo assoluto** della funzione.

### Relativo

Data una funzione $y = f(x)$, definita in un intervallo $[a;b]$, $x_0$ è un **punto di minimo relativo** se esiste un intorno $I$ di $x_0$ tale che:
$$
f(x_0) \leq f(x) \forall x \in I(x_0)
$$

Il valore $f(x_0)$ è detto **minimo relativo** della funzione in $[a;b]$.

## Concavità

### Verso l'alto

Diciamo che in $x_0$ la funzione $f(x)$ ha la **concavità rivolta verso il semiasse positivo delle $y$ (_verso l'alto_)** se esiste un intorno completo $I$ di $x_0$ tale che, per ogni $x$ appartenente all'intorno e diverso da $x_0$, la funzione assume valori maggiori di quelli di $t(x)$ nei punti aventi la stessa ascissa, ossia:
$$
f(x) > t(x) \quad \forall x \in I \land x \neq x_0
$$

### Verso il basso

Diciamo che in $x_0$ la funzione $f(x)$ ha la **concavità rivolta verso il semiasse negativo delle $y$ (_verso il basso_)** se esiste un intorno completo $I$ di $x_0$ tale che, per ogni $x$ appartenente all'intorno e diverso da $x_0$, la funzione assume valori minori di quelli di $t(x)$ nei punti aventi la stessa ascissa, ossia:
$$
f(x) < t(x) \quad \forall x \in I \land x \neq x_0
$$

# Integrali indefiniti

## Primitiva

Una funzione $F(x)$ è una **primitiva** della funzione $f(x)$ definita in un intervallo $[a;b]$ se $F(x)$ è derivabile in tutto $[a;b]$ e la sua derivata è $f(x)$:
$$
F'(x) = f(x)
$$

## Integrale indefinito

L'**integrale indefinito** di una funzione $f(x)$ è l'insieme di tutte le primitive $F(x) + c$ di $f(x)$, con $c$ numero reale qualunque.

Si indica con $\int f(x) \, dx$.

## Condizione sufficiente di integrabilità

Se una funzione è continua in $[a;b]$, allora ammette primitive nello stesso intervallo.

## Proprietà dell'integrale indefinito

### Prima proprietà di linearità

L'integrale indefinito di una somma di funzioni integrabili è uguale alla somma degli integrali indefiniti delle singole funzioni:
$$
\int [ f(x) + g(x) ] \, dx = \int f(x) \, dx + \int g(x) \, dx
$$

### Seconda proprietà di linearità

L'integrale del prodotto di una costante per una funzione integrabile è uguale al prodotto della costante per l'integrale della funzione:
$$
\int k \cdot f(x) \, dx = k \cdot \int f(x) \, dx
$$

## Integrali indefiniti immediati

$$
\begin{aligned}
	\int x^\alpha \, dx &= \frac{x^{\alpha + 1}}{\alpha + 1} + c, \qquad \text{con } \alpha \in \mathbb{R} \land \alpha \neq -1 \\
	\int e^x \, dx &= e^x + c \\
	\int \sin x \, dx &= -\cos x + c \\
	\int \cos x \, dx &= \sin x + c \\
	\int \frac{1}{\cos^2 x} \, dx &= \tan x + c \\
	\int \frac{1}{\sin^2 x} \, dx &= -\cot x + c \\
	\int \frac{1}{\sqrt{1-x^2}} \, dx &= \arcsin x + c \\
	\int \frac{1}{1+x^2} \, dx &= \arctan x + c
\end{aligned}
$$

## Integrazione per parti

$$
\int f(x) \cdot g'(x) \, dx = f(x) \cdot g(x) - \int f'(x) \cdot g(x) \, dx
$$

# Integrali definiti

## Definizione di integrale definito

### Trapezoide

Dati una funzione $y=f(x)$ e un intervallo chiuso e limitato $[a;b]$ nel quale la funzione è _continua e positiva_ (o nulla), il **trapezoide** è la figura piana delimitata dall'asse $x$, dalle rette $x=a$ e $x=b$ e dal grafico di $f(x)$.
Si tratta di un quadrilatero mistilineo di vertici:

- $A(a;0)$
- $B(b;0)$
- $C(b;f(b)$
- $D(a;f(a)$

Viene chiamato trapezoide perchè somiglia a un trapezio con le basi parallele all'asse $y$.

L'area $S$ di un trapezoide non può essere calcolata in modo elementare, ma è possibile approssimarla per eccesso e per difetto.

Con $|b-a| \to 0$, le approssimazioni di $S$ tendono allo stesso numero.

Sommando tutte le approssimazioni si ottiene l'integrale definito

### Definizione

Data una funzione $f(x)$ continua in $[a;b]$, l'**integrale definito** esteso all'intervallo $[a;b]$ è il valore comune del limite per $n \to + \infty$ delle due successioni $s_n$ per difetto e $S_n$ per eccesso.

## Calcolo dell'integrale definito

Data una funzione $f(x)$ continua in $[a;b]$:
$$
\int_a^b f(x) \,dx = \big{[}\upvarphi(x)]_a^b = \upvarphi(b) - \upvarphi(a)
$$

## Teorema della media

Se $f(x)$ è una funzione continua in un intervallo $[a;b]$, esiste almeno un punto $z$ dell'intervallo tale che:
$$
\int_a^b f(x) \,dx = (b-a) \cdot f(z) \qquad \text{con } z \in [a;b]
$$

Quindi:
$$
\frac{\int_a^b f(x) \, dx}{b-a} = f(z)
$$

Questo è il **valore medio** della funzione $f(x)$

## Teorema fondamentale del calcolo integrale

Se una funzione $f(x)$ è continua in $[a;b]$, allora esiste la derivata della sua funzione integrale
$$
F(x) = \int_a^x f(t) \,dt
$$
per ogni punto $x$ dell'intervallo $[a;b]$ ed è uguale a $f(x)$, cioè:
$$
F'(x) = f(x)
$$
ovvero $F(x)$ è una primitiva di $f(x)$.

## Calcolo dell'area delimitata dai grafici di due funzioni

Siano $f(x)$ e $g(x)$ due funzioni continue definite nello stesso intervallo $[a;b]$, con $f(x) \geq g(x)$, per ogni $x \in [a;b]$, i cui grafici racchiudano una superficie; allora l'area $S$ della superficie è data da:
$$
S = \int_a^b [f(x) - g(x)] \, dx
$$

## Calcolo del volume di un solido di rotazione

Dato il trapezoide esteso all'intervallo $[a;b]$, delimitato dal grafico della funzione $y = f(x)$ (positiva o nulla), dall'asse $x$ e dalle rette $x = a$ e $x = b$, il **volume del solido di rotazione** che si ottiene ruotando il trapezoide intorno all'asse $x$ di un giro completo è:
$$
V = \pi \cdot \int_a^b f^2(x) \, dx
$$

## Calcolo del volume tramite medoto delle sezioni

Se di un solido conosciamo la funzione:
$$
\text{area della sezione in }x = S(x)
$$
è possibile calcolare il volume del solido utilizzando la formula:
$$
V = \int_a^b S(x) \, dx
$$

## Integrale di $f$ con un numero finito di discontinuità in $[a;b]$

Data una funzione $f(x)$ definità in un intervallo $[a;b] - d$ (dove $d$ è punto di discontinuità):
$$
\int_a^b f(x) \, dx = \lim_{k \to d^-} \int_a^k f(x) \, dx + \lim_{k \to d^+} \int_k^b f(x) \, dx
$$

## Integrale di $f$ in un intervallo illimitato

$$
\int_a^{+\infty} f(x) \, dx = \lim_{k \to +\infty} \int_a^k f(x) \, dx
$$

$$
\int_{-\infty}^a f(x) \, dx = \lim_{k \to -\infty} \int_k^a f(x) \, dx
$$

# Applicazioni degli integrali alla fisica

## Posizione, velocità e accelerazione

In un moto rettilineo, in un istante $t$:
$$
\begin{aligned}
	s(t) &			& \text{posizione;} \\
	v(t) &= s'(t)	& \text{velocità;} \\
	a(t) &= v'(t) = s''(t)	& \text{accelerazione.}
\end{aligned}
$$

Pertanto, nota l'accelerazione in funzione del tempo $t$, per determianre la velocità e la legge del moto:
$$
\begin{aligned}
	v(t) - v(t_0) &= \int_{t_0}^t a(z) \, dz & &\rightarrow & &v(t) = v(t_0) +  \int_{t_0}^t a(z) \, dz \\
	s(t) - s(t_0) &= \int_{t_0}^t v(z) \, dz & &\rightarrow & &s(t) = s(t_0) +  \int_{t_0}^t v(z) \, dz
\end{aligned}
$$

## Lavoro di una forza

Consideriamo una forza avente per direzione costante una retta $r$ e intensità variabile al variare del punto di applicazione (come una molla).
Indicando con $x$ l'ascissa del punto di applicazione, $F(x)$ è l'intensità della forza.

Il lavoro della forza per lo spostamento del punto di applicazione può essere calcolato con:
$$
L = \int_a^b F(x) \, dx
$$

## Quantità di carica

L'intensità di una corrente è la quantità di carica che attraversa la sezione di un conduttore in una unità di tempo.
Per esprimere l'intensità istantanea nell'istante $t$ si utilizza la derivata della funzione $q(t)$, che lega la quantità di carica al tempo:
$$
i(t) = q'(t)
$$

Se vogliamo determinare la quantità di carica che attraversa la sezione nell'intervallo di tempo da $t_0$ a $t_1$:
$$
Q = \int_{t_0}^{t_1} i(t) \, dt
$$