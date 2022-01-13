[← Home](../README.md)    

# 2021

1. Quel objectif de sécurité garantit la cryptographie symétrique ?  
- [ ] Authentification 
- [ ] Confidentialité 
- [ ] Authenticité 
 
2. Quel mode de chiffrement chiffre le message bit par bit et arrive à traiter des données de longueur quelconque 
sans avoir à les découper ?   
- [] Chiffrement symétrique par bloc 
- [] Chiffrement asymétrique 
- [] Chiffrement symétrique par flux 
 
3. Quelle opération n’est pas utilisée dans les cryptosystèmes symétriques ?  
- [] Transposition de bits 
- [] OU exclusif (XOR)  
- [] Logarithme discret 
 
4. En utilisant un cryptosystème asymétrique, quelle clé utilise-t-on pour signer un message ?  
- [] La clé privée du destinataire   
- [] La clé privée de l’émetteur  
- [] La clé publique du récepteur  
 
5. SSO est l’abréviation de : 
- [] Single Signature On  
- [] Single Sign On 
- [] Sign Single Once  
 
6. KDC est l’abréviation de : 
- [] Key Decentralized centre  
- [] Key Distribution Center 
- [] Kerberos Distributed Center   
 
7. Dans le protocole Kerberos, quel service du KDC est en charge de délivrer le TGT (Ticket Granting Ticket) ?    
- [] Authentication service (AS) 
- [] Ticket Granting Service (TGS) 
- [] Ticket Service (TS) 
 
8. La suite cryptographique ci-dessous est-elle écrite correctement ? 
TLS_ECDHE_AES_128_GCM_WITH_RSA_SHA256 
- [] Oui 
- [] Non  
Justifiez votre réponse   
 
9. Quel procédé permet le traitement des données sans avoir à les déchiffrer au préalable ?  
- [] Chiffrement homomorphe  
- [] Chiffrement de bout en bout  
- [] Chiffrement d’enveloppe 
 
10. Dans quel système de communication, seules les personnes qui communiquent peuvent lire les messages 
échangés ?  
- [] Chiffrement homomorphe  
- [] Chiffrement de bout en bout 
- [] Chiffrement à seuil  
 
11. Quelle est la particularité de la signature aveugle ?   
- [] Elle est signée par une entité secrète 
- [] Elle est effectuée sur un document qui a été masqué auparavant 
- [] C’est une signature qu’on ne peut pas vérifier  
 
12. Qu’est-ce qu’une clé éphémère ?    
- [] Une clé qu’on peut utiliser pour la signature mais pas pour le chiffrement 
- [] Une clé qui sera détruite après utilisation 
- [] Une clé publique  
 
Attention : Les quatre questions suivantes concernent uniquement le groupe LS2 
9. Quel procédé permet le traitement des données sans avoir à les déchiffrer au préalable ?  
- [] Chiffrement homomorphe  
- [] Chiffrement de bout en bout  
- [] Chiffrement d’enveloppe 
 
10. Dans quel système de communication, seules les personnes qui communiquent peuvent lire les messages 
échangés ?  
- [] Chiffrement homomorphe  
- [] Chiffrement de bout en bout 
- [] Chiffrement à seuil  
 
11. Quel  mode  de  chiffrement  permet  de  diviser  un  message  en  plusieurs  blocs.  Ces  blocs  sont  ensuite 
chiffrés séparément les uns après les autres ? 
- [] CBC 
- [] ECB 
 
12. Quel(s) objectif(s) de sécurité garantit un HMAC (keyed-hash message authentication code) ?  
- [] Confidentialité  
- [] Intégrité  
- [] Intégrité et Authentification  
 
1. Donnez la définition d’une fonction de hachage.
 
2. Quels sont les services externes nécessaires au bon fonctionnement de Kerberos ? 
3. Quelles sont les trois étapes de la phase Handshake du protocole SSL/TLS ? 
 
 
 
 
 
 
 
4. Quel processus de chiffrement est le plus lent,  celui  d’un  cryptosystème  symétrique  ou  celui  d’un 
cryptosystème asymétrique ? justifiez votre réponse.
 
 
5. Dans  quel  ordre  se  font  les  opérations  suivantes :  chiffrement,  signature  numérique  et  hachage ?  justifiez 
votre réponse.  
 
 
 
 
6. Peut-on signer un message en utilisant un cryptosystème symétrique ? Justifiez votre réponse.
 
 
7. Que fait la commande OpenSSL suivante ?   
OpenSSL dgst -MD5 Texte.txt  -out Text2.txt
 
 
 
8. En utilisant la boîte à outils OpenSSL pour générer une clé publique RSA, a-t-on besoin de préciser la taille de 
la clé souhaitée ? Justifiez votre réponse. 
 
 
 
9. Expliquez les étapes, de la demande à l’obtention, d’un certificat numérique en mettant en avant les entités 
concernées à chaque étape (utilisez un schéma de préférence). Quelle clé est utilisée pour signer le certificat 
numérique (nature de la clé + propriétaire) ? 




 
 
 
 
Le tableau suivant représente les étapes d’un cryptosystème :   
 Alice Bob 
Etape 1 Alice et Bob choisissent ensemble deux valeurs p et α  
Etape  2 Alice choisit secrètement a et envoie A = α a mod p 
à Bob 
Bob choisit secrètement b et envoie B = α b mod p 
à Alice 
 
Etape 3 Alice calcule B a mod p Bob calcule A b mod p 
 
1. Quelle est l’objectif de ce cryptosystème ? 
 
 
 
 
2. Que représente chaque valeur : a, b, A, B, B a mod p et A b mod p ?  

 
 
 
 
 
 
 
 
3. Une personne se trouvant entre Alice et Bob, peut-elle retrouver les valeurs a et b ?   
- [] Oui               
- [] Non  
Justifiez votre réponse 




 
 
  
