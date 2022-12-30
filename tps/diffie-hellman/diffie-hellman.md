# Diffie Hellman key exchange

## Descrizione
Viene utilizzato per negoziare una chiave segreta senza trasmetterla.

## Procedimento
- $g = 265$
- $P =$ primo("grande") _segreto_
- $a =$ casuale
- $b =$ casuale
- $A = g^a \% p$
- $B = g^b \% p$

### Generazione chiavi intermedie


```python
from random import randint

# CLIENT A

g = 265
P = 2**127-1
a = randint(100, 10000)

A = ( g**a ) % P

# trasmessi:
print(g)
print(P)
print(A)
```

    265
    170141183460469231731687303715884105727
    65762947159903478482237843901310241724



```python
# CLIENT B

b = randint(100, 10000)

B = ( g**b ) % P

print(B)
```

    92970624912426329491514596993598347898


### Generazione chiave


```python
# CLIENT A
secretA = ( B**a ) % P

print(secretA)
```

    112346438519136498128656281459096927081



```python
# CLIENT B
secretB = ( A**b ) % P

print(secretB)
```

    112346438519136498128656281459096927081

