# Sceau CertifiKation

## Définition

Le Sceau CertifiKation est la preuve exportable produite à partir d’un Profil de Calibre.

Il ne doit pas contenir toutes les réponses ni tous les détails de session. Il doit contenir l’essentiel nécessaire pour attester une compétence.

## Contenu recommandé

- personne ou identifiant ;
- domaine ;
- compétence ;
- niveau confirmé ;
- date ;
- durée de validité ;
- version des règles ;
- source XKaliber ;
- marge de confiance ;
- conditions de validité ;
- lien vers explication ou audit autorisé ;
- statut : actif, expiré, révoqué, contesté, corrigé.

## Statuts

### Actif

La preuve est valide.

### Expiré

La preuve doit être recalibrée.

### Contesté

Une révision est en cours.

### Corrigé

Un changement a été appliqué après révision.

### Révoqué

La preuve ne doit plus être utilisée.

## Handoff vers K-Port

Lorsqu’un Sceau CertifiKation doit contribuer à EkoH, il est transmis à **K-Port**, pas directement au moteur de scoring EkoH.

Le handoff devrait préserver au minimum :

- l’identifiant du Sceau et sa provenance ;
- la personne concernée ;
- le domaine et la compétence ;
- le niveau confirmé ;
- la confiance issue de XKaliber ;
- les dates d’évaluation, d’émission et d’expiration ;
- la version des règles ;
- le statut courant ;
- les conditions et limites de validité ;
- le consentement ;
- une référence d’audit ou de vérification.

K-Port vérifie la provenance, le statut, la portée, l’identité, le consentement et le mapping EkoH. Il ne refait pas l’évaluation XKaliber et ne modifie pas le niveau confirmé.

Toute correction, expiration ou révocation du Sceau doit pouvoir être propagée à K-Port afin qu’EkoH puisse réévaluer l’impact réputationnel si nécessaire.

## Limite

Un Sceau CertifiKation ne doit pas être utilisé comme preuve hors de son domaine, de son niveau et de son contexte. Il ne constitue pas, à lui seul, un score ou une réputation EkoH.
