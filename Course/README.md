[← Home](../README.md)    
[→]()

# Cours

## Chiffrement symétrique
- 😃 Simple à mettre en oeuvre
- 😃 Chiffrement rapide
- 😡 L'échange de clé
#### Chiffrement par flux (Stream Cipher)
Bit à bit, communication temps réel (Bluetooth, RC4)

#### Chiffrement par bloc (Bloc Cipher)
Bloc par bloc taille fixe (DES, AES)

### DES
Text ➡ Permutation ➡ Substitution (k fois) ➡ Permutation inverse ➡ Texte

Attaque par ordinateur très simple

### AES
Se base sur un système de matrice

- Text ➡ ...
    - (SubBytes ➡ ShiftRows ➡ MixColumns ➡ AddRoundKey) x Nr-1
    - SubBytes ➡ ShiftRows ➡ AddRoundKey ➡ ...   
- ... ➡ CipherText

## Chiffrement asymétrique
- 😃 Résout l'échange de clé
- 😡 Chiffrement lent
- 😡 Coûteux en ressources

### Fonctionnement 
- Clé publique, privée
- Fonction à sens unique
- Problèmes non polynomiaux

### Problèmes non polymoniaux
#### Factorisation de grand nombre
- RSA 
- Rabin
#### Logarithme discret
- El Gamal
- Diffie-helman
#### Courbe elliptique
- ECDH
- ECDSA

### RSA
1. `p`, `q` nombres premiers. `n = p * q`
2. `e` (exposant de chiffrement) premier avec  `φ(n) = (p - 1)(q - 1)`
3. `d` inverse de `e modulo φ(n)`
- Clé publique `(n, e)` 
- Clé privée `(p, q, d)`
4. Alice **chiffre** un message `x`: `y ≡ x^e mod n`
5. Bob **déchiffre** `y`: `x ≡ y^d mod n`

### Signature
#### Alice
- Clé privée (p<sub>a</sub>, q<sub>a</sub>, d<sub>a</sub>)
- Clé publique (n<sub>a</sub>, e<sub>a</sub>)

#### Signature d'Alice
<!-- $$
Sign(x) \equiv y \equiv x^{d_{a}} \mod n_{a}
$$ --> 

<div align="center" style="background: white;"><img style="background: white;" src="https://render.githubusercontent.com/render/math?math=Sign(x)%20%5Cequiv%20y%20%5Cequiv%20x%5E%7Bd_%7Ba%7D%7D%20%5Cmod%20n_%7Ba%7D"></div>

#### Message signé
(x, Sign(x))

#### Vérification de la signature
<!-- $$
y^{e_{a}} \equiv x \mod n_{a}
$$ --> 

<div align="center" style="background: white;"><img style="background: white;" src="https://render.githubusercontent.com/render/math?math=y%5E%7Be_%7Ba%7D%7D%20%5Cequiv%20x%20%5Cmod%20n_%7Ba%7D"></div>

## Cryptographie moderne
### Fonction de hachage
Fonction à sens unique:    
**message de longueur arbitraire** → **empreinte numérique de taille fixe**

- MD5
- SHA-1
- SHA-256