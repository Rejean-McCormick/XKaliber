# Intégration avec Konnaxion

## Relation entre les modules

```text
KonnectED / parcours d’apprentissage
        ↓
     XKaliber
        ↓
Profil de Calibre
        ↓
  CertifiKation
        ↓
      K-Port
        ↓
       EkoH
        ↓
SmartVote / autres usages gouvernés
```

Le portfolio KonnectED peut conserver et afficher la preuve, mais il ne remplace pas K-Port comme passerelle d’évidence lorsqu’une preuve doit influencer EkoH.

## Rôles

### KonnectED

Développe les compétences par parcours, cours, activités et portfolio.

### XKaliber

Mesure le calibre réel par épreuve adaptative et produit un résultat de compétence source-authoritatif.

### CertifiKation

Atteste une compétence confirmée et produit une preuve exportable, bornée par domaine, niveau, date et conditions de validité.

### K-Port

Agit comme **passerelle canonique d’évidence vers EkoH**. Il reçoit notamment les preuves XKaliber / CertifiKation, vérifie leur provenance, leur statut, leur portée, leur association à la bonne personne, leur consentement et leur mapping vers les domaines EkoH.

K-Port **ne refait pas l’évaluation XKaliber et ne recalcule pas le niveau confirmé**. XKaliber reste l’autorité source pour la performance observée.

### EkoH

Reçoit de K-Port des signaux admissibles et bornés par domaine. EkoH reste la seule autorité qui décide de l’impact sur la réputation, applique les paramètres de scoring et conserve l’historique des changements.

### SmartVote

Peut utiliser certains signaux de compétence ou de réputation fournis par les interfaces gouvernées d’EkoH, si les règles publiques le permettent. SmartVote ne reçoit pas directement les résultats bruts XKaliber.

### Konnaxion

Rend la Table ronde opérante : apprentissage, compétence, preuve, réputation, délibération, décision et action peuvent se relier sans confondre leurs autorités.

## Principe d’échange

XKaliber ne doit pas partager plus que nécessaire et ne doit pas contourner K-Port pour un usage EkoH.

| Destination | Donnée recommandée | Autorité |
|---|---|---|
| KonnectED | profil complet ou pédagogique | XKaliber pour le résultat |
| CertifiKation | niveau confirmé et éléments nécessaires à l’attestation | XKaliber / CertifiKation |
| K-Port | preuve structurée, provenance, statut, confiance, limites et consentement | XKaliber comme source; K-Port pour l’admissibilité |
| EkoH | aucun flux direct depuis XKaliber; signal préparé par K-Port | EkoH pour le scoring |
| SmartVote | aucun flux direct depuis XKaliber; indicateur gouverné issu d’EkoH | règles SmartVote / EkoH |
| Konnaxion public | résumé seulement si consentement et politique de visibilité | politique Konnaxion |

## Phrase d’intégration

**XKaliber mesure la compétence. CertifiKation l’atteste. K-Port qualifie et route l’évidence. EkoH transforme l’évidence admissible en réputation. Konnaxion utilise ensuite cette réputation selon des règles gouvernées.**
