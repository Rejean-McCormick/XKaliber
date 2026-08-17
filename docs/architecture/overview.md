# Architecture conceptuelle

## Définition

XKaliber est un moteur d’évaluation adaptative qui transforme des performances observées en profils de compétence contextualisés.

Il ne remplace pas CertifiKation. Il fournit la mesure qui permet à CertifiKation d’attester.

Lorsqu’une preuve XKaliber doit contribuer à la réputation EkoH, elle ne contourne pas la couche d’évidence. Le Profil de Calibre ou le Sceau CertifiKation est transmis à **K-Port**, qui agit comme passerelle canonique d’évidence vers EkoH. K-Port vérifie la provenance, le statut, la portée, le consentement et le mapping de domaine sans recalculer la performance évaluée par XKaliber.

## Chaîne conceptuelle

```text
Parcours d’apprentissage
→ Demande d’évaluation
→ Scan initial
→ Épreuve adaptative
→ Profil de Calibre
→ Sceau CertifiKation
→ Portfolio KonnectED, si souhaité
→ Handoff de preuve vers K-Port
→ Contrôle de provenance, statut, portée et consentement par K-Port
→ Signal admissible vers EkoH
→ Calcul de réputation par EkoH
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

Ces fonctions appartiennent à KonnectED, CertifiKation, **K-Port**, EkoH, SmartVote, Orgo ou d’autres modules.

En particulier, XKaliber ne doit pas devenir une seconde couche d’intake ou de scoring réputationnel : K-Port centralise l’évidence admissible et EkoH reste l’autorité de scoring.

## Sorties

XKaliber produit principalement :

- un profil ;
- des preuves structurées ;
- des recommandations ;
- des traces ;
- des paquets d’évidence bornés par domaine destinés à CertifiKation et, lorsque requis, à K-Port.
