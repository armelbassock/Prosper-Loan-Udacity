
# JEU DE DONNEES PROSPER LOAN

## INTRODUCTION

Un pret est le fait pour un établissement de crédit, de proposer une solution de financement, en mettant à disposition des fonds à un bénéficiaire, sans en exiger le remboursement immédiat. Dans ce document, nous allons étudier un ensemble de données de pret, fournit par Prosper.

Ce jeu de données comprend un ensemble 113 937 prêts avec 81 variables sur chaque prêt, y compris le montant du prêt, le taux de l'emprunteur (ou taux d'intérêt), le statut actuel du prêt, le revenu de l'emprunteur, et bien d'autres.

**Exploitation:** Dans le but de retirer des informations utiles de ce jeu de données, nous nous posons les questions suivantes :᷆

* Quels facteurs affectent le statut du résultat d'un pret ?
* QU'est ce qui affecte l'APR ou le taux d̀intéret de l'emprunteur ?
* Existe-t-il des différences entre les prets en fonction de l'importance du montant initialement emprunté ?
* Afin de repondre a ces questions, nous avons exploré notre dataset à travers plusieurs caractéristiques. Les caracteristiques   d'interet principales étant :

* LoanStatus -- statut du pret
* BorrowerAPR -- taux annuel effectif global de l'emprunteur
* BorrowerRate -- Taux d'interet de l'emprunt pour ce pret
* LenderYield -- Rendement du preteur
* LoanOriginalAmount -- montant initial du pret

## ANALYSE EXPLORATOIRE

Dans l'analyse exploratoire, nous avons effectué un nettoyage des données. Puis nous avons effectué des explorations sur nos variables d̀intéret.

### Analyse univariée

Les  variables que nous avons observés sont _loanstatus, borrowerAPR, LoanOriginalAmount, ListingCategory, DebtToIncomeRatio et IncomeRange_. Nous avons observé au terme de cette analyse que les credits présentent un risque faible et sont surtout demander dans l'optique d'une consolidation des dettes

### Analyse bivariée

A partir de certaines des variables précédentes nous avons essayé de déduire des relations des variables d'intéret que sont _LoanStatus (relation avec LOA, EmployedStatus, IncomeRange, LP_CP) et BorrowerAPR (BorrowerRate, LenderYield, BorrowerState, Occupation) _. Nous avons observer une forte corrélation entre BorrowerAPR et les variables LenderYield et BorrowerRate. De plus les prets ayant un statut de pret remboursé ou en voie de remboursement sont dans ube tranche de revenus modéré̀ment élevée
### Analyse multivariée

A partir des analyses multivariées on a observer le statut d̀un pret en fonction de l'APR et de l'Occupation et on a observé que les ingénieurs electricien en phase finale de remboursement ont l'APR le plus élevé.


## ANALYSE  EXPLICATIVE

Nous avons présenté un slide avec les diagrammes les plus pertinents de notre analyse.
Pour cela nous avons utilisé 3 visualisations clés:

### visualisation 1

Le premier apercu est un diagramme en secteur de la colonne 'IncomeRange'. Il avait pour but de présenter les tranches de revenu ayant la plus grande fréquence de prets.

#### Résultat obtenu

On constate que les personnes à revenus moyen donc compris entre **25 000 et 75 000 dollars** sont les plus demandeuses de pret.


### visualisation 2

Le deuxième apercu est un diagramme à barres groupé ayant en abscisse 'LoanStatus' et qui attribue à chaque couleur de barre une valeur dans la colonne 'IncomeRange'. Il avait pour but de déterminer quels sont les tranches de revenus dont les prets sont en cours de rembousement ou ont déjà été remboursés.

#### Résultat obtenu

On constate que les tranches de revenu comprises entre **25 000 et 75 000 dollars** sont également de loin les plus présente dans les catégories de pret complétés ou en cours de remboursement.

### visualisation 3

Le troisième apercu est un diagramme à barres groupé horizontale ayant en abscisse 'BorrozerAPR', en ordonnée 'Occupation' et qui attribue à chaque couleur de barre une valeur dans la colonne 'LoanStatus'. Il avait pour but de déterminer quels sont parmis les 10 occupations ayant des  taux d'emprunt les plus bas, quelle est celle dont on pourrait améliorer le taux.

#### Résultat obtenu

De nos observations on constate que le taux annuel de l'emprunt est plus élevé pour les **ingénieurs électriciens** en phase final du processus de remboursement. Donc améliorer leur taux pourrait les aider à rembourser plus vite.

## CONCLUSION

Apres avoir effectué une analyse exploratoire sur notre ensemble de données, il en est ressorti que des paramètres présents dans 
le jeu de données, l'occuppation et la tranche de revenus sont des paramètres intéressants pour nos études.
Dans la partie présentation᷆, nous présentons 3 visuels qui nous permettent de déterminer ce qui peut influencer le statut d'un pret ou le taux d'un emprunteur.