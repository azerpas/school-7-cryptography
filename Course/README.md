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
