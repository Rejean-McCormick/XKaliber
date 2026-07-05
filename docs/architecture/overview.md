# Architecture conceptuelle

## Définition

XKaliber est un moteur d’évaluation adaptative qui transforme des performances observées en profils de compétence contextualisés.

Il ne remplace pas CertifiKation. Il fournit la mesure qui permet à CertifiKation d’attester.

## Chaîne conceptuelle

```text
Parcours d’apprentissage
→ Demande d’évaluation
→ Scan initial
→ Épreuve adaptative
→ Profil de Calibre
→ Sceau CertifiKation
→ Portfolio KonnectED
→ Signal possible vers EkoH
→ Usage gouverné dans Konnaxion
```

## Composants conceptuels

### Domaine

Champ de compétence : programmation, soins, gouvernance, médiation, mécanique, enseignement, etc.

### Compétence

Capacité précise à évaluer dans un domaine.

### Niveau

Degré de complexité ou de responsabilité.

### Item ou tâche

Élément d’épreuve : question, simulation, étude de cas, production, jugement, geste, résolution.

### Session

Évaluation vécue par une personne à un moment donné.

### Moteur adaptatif

Logique qui choisit la suite de l’épreuve selon la performance.

### Profil de Calibre

Rapport final de compétence.

### Sceau CertifiKation

Preuve exportable attestant un niveau confirmé.

## Frontières

XKaliber ne devrait pas contenir toute la logique de :

- gestion complète des cours ;
- réseau social ;
- gouvernance globale ;
- vote ;
- embauche ;
- gestion RH ;
- identité permanente.

Ces fonctions appartiennent à KonnectED, CertifiKation, EkoH, SmartVote, Orgo ou d’autres modules.

## Sorties

XKaliber produit principalement :

- un profil ;
- des preuves ;
- des recommandations ;
- des traces ;
- des signaux bornés par domaine.
