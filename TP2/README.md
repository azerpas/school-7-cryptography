[← Home](../README.md)    
[→]()

# TP2

# HTTPS

## SSL
Protocole pour communiquer de façon sécurisée sur TCP/IP.
### Steps
1. **Handshake**: client - serveur identification, déf système de chiffrement et clé utilisée.
2. **Communication**: échange de données chiffrées, signées

TLS est une évolution de SSL.

## OpenSSL 
Toolkit qui permet d'implémenter SSL et TLS en C. 
- Création de clés RSA, DSA
- Création de certificats X509
- Calcul d'empreintes MD5 SHA
- Chiffrement et déchiffrement DES IDE
- ...