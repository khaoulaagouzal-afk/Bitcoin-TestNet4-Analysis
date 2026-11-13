# Analyse d'une transaction Bitcoin sur TestNet4

**Réalisé par :** Khaoula Agouzal  
**Formation :** Master FinTech  
**Établissement :** FSJES Marrakech – Université Cadi Ayyad

## 1. Introduction

Bitcoin est une cryptomonnaie qui fonctionne grâce à une technologie appelée blockchain. Cette technologie permet d'enregistrer les transactions dans un registre numérique partagé et sécurisé.

Dans ce projet, nous allons étudier le fonctionnement d'une transaction Bitcoin réalisée sur le réseau TestNet4.

## 2. Présentation de TestNet4

TestNet4 est un réseau de test de Bitcoin. Il permet aux utilisateurs d'effectuer des transactions sans utiliser de véritables bitcoins.

Il fonctionne de manière similaire au réseau Bitcoin principal, mais utilise des bitcoins de test qui n'ont pas de valeur monétaire réelle.

## 3. Fonctionnement d'une transaction

Une transaction Bitcoin permet de transférer des bitcoins d'une adresse à une autre.

Elle contient principalement :

- **Inputs (entrées) :** les bitcoins utilisés pour financer la transaction.
- **Outputs (sorties) :** les montants envoyés aux destinataires.
- **Transaction Fee (frais) :** le montant payé aux mineurs pour le traitement de la transaction.

## 4. Comprendre les UTXO

UTXO signifie Unspent Transaction Output.

Il représente une sortie de transaction qui n'a pas encore été dépensée.

Bitcoin utilise ce système pour suivre les montants disponibles et permettre la création de nouvelles transactions.

## 5. Confirmations

Une confirmation apparaît lorsqu'une transaction est incluse dans un bloc validé par le réseau.

Plus le nombre de confirmations augmente, plus la transaction est considérée comme difficile à modifier.

## 6. Conclusion

L'utilisation de Bitcoin TestNet4 permet de comprendre le fonctionnement des transactions blockchain dans un environnement de test.

Cette expérience nous aide à mieux comprendre les entrées, les sorties, les frais, les UTXO et les confirmations.

## 7. Outils utilisés

- Bitcoin TestNet4
- Wasabi Wallet
- GitHub Desktop
- GitHub
- Assistance IA pour l'organisation et la rédaction du contenu.

## 8. Analyse pratique de deux transactions Bitcoin sur TestNet4

Cette partie présente l'analyse de deux transactions réalisées sur le réseau Bitcoin TestNet4 à l'aide de l'explorateur Mempool.space.

### 8.1 Première transaction : réception de bitcoins

**TXID :**
b7c34106c65f31044b065ec7e22a5974bcafaec1c19467156ea00e11203c0ae3

- Date : 24 octobre 2026 à 19:52:43
- Statut : Confirmed
- Délai de confirmation : 1 jour
- Type : SegWit
- Nombre d'Inputs : 1
- Nombre d'Outputs : 2
- Frais : 167 satoshis
- Fee rate : 1.02 sat/vB
- Taille : 246 bytes
- Virtual size : 164.25 vB
- Weight : 657 WU

**Input :**
- 34.90215897 tBTC

**Outputs :**
- Sortie 1 : 0.00208885 tBTC
- Sortie 2 : 34.90006845 tBTC

**Interprétation :**

Cette transaction utilise une entrée et crée deux sorties. La première sortie correspond à un montant de 0.00208885 tBTC, utilisé comme entrée dans la deuxième transaction. La deuxième sortie peut correspondre à la monnaie rendue (Change).

Les frais de transaction sont de 167 satoshis.

### 8.2 Deuxième transaction : envoi de bitcoins

**TXID :**
3bb9132ca25e7f74bd05353e2db85e2f343924cfb0d9d2400f6d150c098dcc31

- Date : 24 octobre 2026 à 19:52:43
- Statut : Confirmed
- Délai de confirmation : 1 jour
- Nombre d'Inputs : 1
- Nombre d'Outputs : 2
- Frais : 1 716 satoshis
- Fee rate : 12.1 sat/vB
- Taille : 193 bytes
- Virtual size : 142 vB
- Weight : 568 WU

**Input :**
- 0.00208885 tBTC

**Outputs :**
- Sortie 1 : 0.00100000 tBTC
- Sortie 2 : 0.00107169 tBTC

**Interprétation :**

Cette transaction utilise le montant de 0.00208885 tBTC reçu dans la première transaction.

Elle répartit ce montant entre deux sorties : 0.00100000 tBTC envoyés et 0.00107169 tBTC correspondant à la monnaie restante (Change).

Les frais de transaction sont de 1 716 satoshis.

### 8.3 Relation entre les deux transactions et fonctionnement des UTXO

Les deux transactions sont directement liées.

La première transaction crée une sortie de 0.00208885 tBTC. Cette sortie est ensuite utilisée comme entrée dans la deuxième transaction.

Cela illustre le fonctionnement du modèle UTXO (Unspent Transaction Output) de Bitcoin.

Une sortie non dépensée peut être utilisée comme entrée dans une nouvelle transaction.

### 8.4 Comparaison des frais

La première transaction présente des frais de 167 satoshis, avec un taux de 1.02 sat/vB.

La deuxième transaction présente des frais de 1 716 satoshis, avec un taux de 12.1 sat/vB.

La deuxième transaction a donc des frais plus élevés, notamment en raison de son taux de frais par unité de taille virtuelle plus important.

### 8.5 Conclusion de l'analyse pratique

Cette expérience pratique a permis d'observer deux transactions réelles sur Bitcoin TestNet4.

Elle montre comment les bitcoins sont reçus, dépensés et répartis entre plusieurs sorties.

Elle permet également de comprendre le rôle des frais de transaction et le fonctionnement du modèle UTXO.

Les deux transactions ont été confirmées sur le réseau TestNet4.

Les montants utilisés sont des bitcoins de test (tBTC) et n'ont pas de valeur monétaire réelle.

## 9. Sources

- Explorateur Mempool.space : https://mempool.space/testnet4
- Première transaction : https://mempool.space/testnet4/tx/b7c34106c65f31044b065ec7e22a5974bcafaec1c19467156ea00e11203c0ae3
- Deuxième transaction : https://mempool.space/testnet4/tx/3bb9132ca25e7f74bd05353e2db85e2f343924cfb0d9d2400f6d150c098dcc31
