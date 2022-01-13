[← Home](../README.md)    

# 2021

## 1. Quel objectif de sécurité garantit la cryptographie symétrique ?  
- [ ] Authentification 
- [X] Confidentialité 
- [ ] Authenticité 
 
## 2. Quel mode de chiffrement chiffre le message bit par bit et arrive à traiter des données de longueur quelconque 
sans avoir à les découper ?   
- [ ] Chiffrement symétrique par bloc 
- [ ] Chiffrement asymétrique 
- [X] Chiffrement symétrique par flux 
 
## 3. Quelle opération n’est pas utilisée dans les cryptosystèmes symétriques ?  
- [ ] Transposition de bits 
- [ ] OU exclusif (XOR)  
- [X] Logarithme discret 
 
## 4. En utilisant un cryptosystème asymétrique, quelle clé utilise-t-on pour signer un message ?  
- [ ] La clé privée du destinataire   
- [X] La clé privée de l’émetteur  
- [ ] La clé publique du récepteur  
 
## 5. SSO est l’abréviation de : 
- [ ] Single Signature On  
- [X] Single Sign On 
- [ ] Sign Single Once  
 
## 6. KDC est l’abréviation de : 
- [ ] Key Decentralized centre  
- [X] Key Distribution Center 
- [ ] Kerberos Distributed Center   
 
## 7. Dans le protocole Kerberos, quel service du KDC est en charge de délivrer le TGT (Ticket Granting Ticket) ?    
- [X] Authentication service (AS) 
- [ ] Ticket Granting Service (TGS) 
- [ ] Ticket Service (TS) 
 
## 8. La suite cryptographique ci-dessous est-elle écrite correctement ? 
TLS_ECDHE_AES_128_GCM_WITH_RSA_SHA256 
- [ ] Oui 
- [X] Non  
Justifiez votre réponse   
```
RSA devrait être placé avant AES_128_GCM.
```

## 9. Quel procédé permet le traitement des données sans avoir à les déchiffrer au préalable ?  
- [X] Chiffrement homomorphe  
- [ ] Chiffrement de bout en bout  
- [ ] Chiffrement d’enveloppe 
 
## 10. Dans quel système de communication, seules les personnes qui communiquent peuvent lire les messages 
échangés ?  
- [ ] Chiffrement homomorphe  
- [X] Chiffrement de bout en bout 
- [ ] Chiffrement à seuil  
 
## 11. Quelle est la particularité de la signature aveugle ?   
- [ ] Elle est signée par une entité secrète 
- [X] Elle est effectuée sur un document qui a été masqué auparavant 
- [ ] C’est une signature qu’on ne peut pas vérifier  
 
## 12. Qu’est-ce qu’une clé éphémère ?    
- [ ] Une clé qu’on peut utiliser pour la signature mais pas pour le chiffrement 
- [X] Une clé qui sera détruite après utilisation 
- [ ] Une clé publique  
 
## 11. Quel  mode  de  chiffrement  permet  de  diviser  un  message  en  plusieurs  blocs.  Ces  blocs  sont  ensuite 
chiffrés séparément les uns après les autres ? 
- [X] CBC 
- [ ] ECB    
```Cipher Block Chaining```
 
## 12. Quel(s) objectif(s) de sécurité garantit un HMAC (keyed-hash message authentication code) ?  
- [ ] Confidentialité  
- [ ] Intégrité  
- [X] Intégrité et Authentification  
 
## 1. Donnez la définition d’une fonction de hachage.
Fonction à sens unique qui pour une entrée unique, produit toujours la même chaîne chaîne de caractères de 160 bits.

## 2. Quels sont les services externes nécessaires au bon fonctionnement de Kerberos ? 
- AS: Authentication Service
- TGS: Ticket Granting System

## 3. Quelles sont les trois étapes de la phase Handshake du protocole SSL/TLS ?
- Authentification des serveurs
- Se mettre d'accord sur protocole
- Échanger clés
 
## 4. Quel processus de chiffrement est le plus lent,  celui  d’un  cryptosystème  symétrique  ou  celui  d’un 
cryptosystème asymétrique ? justifiez votre réponse.
```
Asymétrique car il utilise des algorithmes complexes qui nécessite des divisions de très grands nombres et donc de gros calculs. 
```
 
 
## 5. Dans  quel  ordre  se  font  les  opérations  suivantes :  chiffrement,  signature  numérique  et  hachage ?  justifiez 
votre réponse.  
- hachage
- chiffrement
- signature

```
On hash d'abord nos données afin d'obtenir une empreinte qui elle sera chiffrée par la clé privée de l'expéditeur, ce qui consiste en une signature numérique.
```
 
## 6. Peut-on signer un message en utilisant un cryptosystème symétrique ? Justifiez votre réponse.
```
En possèdant la clé privée il est possible de signer un message qui sera ensuite vérifiable par quelqu'un qui possède aussi la clé. 
```
 
## 7. Que fait la commande OpenSSL suivante ?   
OpenSSL dgst -MD5 Texte.txt  -out Text2.txt
```
On hash Texte.txt en utilisant MD5, on sauvegarde le résultat dans Text2.txt
```
 
## 8. En utilisant la boîte à outils OpenSSL pour générer une clé publique RSA, a-t-on besoin de préciser la taille de 
la clé souhaitée ? Justifiez votre réponse. 
```
Non, la taille de clé par défaut sera de 2048 bits.
```
 
## 9. Expliquez les étapes, de la demande à l’obtention, d’un certificat numérique en mettant en avant les entités concernées à chaque étape (utilisez un schéma de préférence). Quelle clé est utilisée pour signer le certificat numérique (nature de la clé + propriétaire) ? 
 
## Alice & Bob 
1. Alice et Bob choisissent ensemble deux valeurs p et α  

### Alice
2. Alice choisit secrètement a et envoie A = α^a mod p 
à Bob.
3. Alice calcule B^a mod p 

### Bob
2. Bob choisit secrètement b et envoie B = α^b mod p 
à Alice 
3. Bob calcule A^b mod p 
 
## 1. Quelle est l’objectif de ce cryptosystème ? 
```
Nous sommes dans un contexte RSA où l'on vise à définir clé publique / privée d'Alice et de Bob.
```
 
 
## 2. Que représente chaque valeur : a, b, A, B, B^a mod p et A^b mod p ?  
- `a` partie de la clé privée d'Alice
- `b` partie de la clé privée de Bob
- `A` signature d'Alice
- `B` signature de Bob
- `B^a mod p` vérification signature de Bob
- `A^b mod p` vérification signature d'Alice
 
## 3. Une personne se trouvant entre Alice et Bob, peut-elle retrouver les valeurs a et b ?   
- [X] Oui               
- [ ] Non  
Justifiez votre réponse 
```
Si les valeurs de a et de b sont faibles, à l'aide de brute-force un attaquant pourrait retrouver les dites valeurs.
```