# Handoff vers K-Port, EkoH et SmartVote

## Principe

XKaliber peut contribuer à la crédibilité par domaine, mais il ne doit ni créer une autorité globale ni écrire directement dans la réputation EkoH.

La chaîne canonique est :

```text
XKaliber
→ Profil de Calibre / résultat confirmé
→ Sceau CertifiKation, lorsque applicable
→ K-Port
→ signal de scoring admissible
→ EkoH
→ usages gouvernés, dont SmartVote lorsque permis
```

**K-Port est la passerelle canonique d’évidence vers EkoH.**

## Paquet d’évidence minimal vers K-Port

Une preuve XKaliber ou CertifiKation transmise à K-Port devrait contenir au minimum :

- identifiant de la personne ou référence d’identité autorisée ;
- `source_module` : `xkaliber` ou `certifikation` ;
- identifiant stable du Profil de Calibre ou du Sceau ;
- domaine ;
- compétence ;
- niveau confirmé ;
- date de l’évaluation ;
- date d’émission de la preuve, si différente ;
- confiance ou marge de confiance ;
- durée de validité ou date d’expiration ;
- version des règles / de l’épreuve ;
- statut : actif, expiré, contesté, corrigé ou révoqué ;
- limites d’usage ;
- consentement et visibilité ;
- référence d’audit ou mécanisme de vérification de provenance.

## Autorité source et contrôle K-Port

Pour une preuve XKaliber valide, K-Port doit distinguer deux responsabilités :

**XKaliber / CertifiKation sont autoritatifs pour :**

- la performance observée ;
- le niveau confirmé ;
- la confiance issue de l’évaluation ;
- les règles et versions ayant produit le résultat ;
- les corrections ou révocations de cette preuve.

**K-Port est autoritatif pour :**

- vérifier que la preuve provient bien de XKaliber / CertifiKation ;
- lier la preuve à la bonne personne ;
- vérifier le statut, l’expiration et les révocations ;
- vérifier les limites et le consentement ;
- prévenir les doublons ;
- mapper ou confirmer la correspondance avec les domaines EkoH ;
- déterminer si l’évidence est admissible au handoff EkoH.

K-Port **ne doit pas refaire l’épreuve, modifier le niveau confirmé ou recalculer la confiance XKaliber**. Toute contestation de la mesure retourne au processus de révision XKaliber / CertifiKation.

## Signal EkoH

XKaliber ne construit pas le score de réputation. K-Port prépare le handoff à partir de l’évidence admissible, puis EkoH décide :

- si la preuve doit avoir un impact ;
- sur quel domaine EkoH ;
- avec quel poids selon ses paramètres ;
- comment la fraîcheur, les autres preuves et les règles de réputation interagissent ;
- comment le changement est consigné dans l’historique de score.

La confiance XKaliber est un **attribut de la preuve**, pas un score EkoH.

## Ce qu’il ne faut pas envoyer par défaut

Ni K-Port, ni EkoH, ni SmartVote ne devraient recevoir par défaut :

- réponses brutes ;
- temps détaillés ;
- erreurs personnelles sensibles ;
- commentaires privés ;
- données non nécessaires ;
- interprétations hors domaine.

## Usage SmartVote

SmartVote peut utiliser des signaux de compétence ou de réputation seulement si :

- le signal provient d’une interface gouvernée d’EkoH plutôt que directement de XKaliber ;
- le domaine du vote correspond au domaine validé ;
- les règles de pondération sont publiques ;
- les lectures non pondérées restent visibles ;
- la personne sait que le signal est utilisé ;
- la communauté peut contester la règle ;
- le signal est limité dans le temps.

## Propagation des changements

Une correction, expiration ou révocation XKaliber / CertifiKation doit pouvoir se propager vers K-Port. K-Port met alors à jour l’état de l’évidence et déclenche, si nécessaire, une réévaluation de l’impact par EkoH. XKaliber ne corrige pas directement un score EkoH.

## Phrase clé

**XKaliber mesure ; K-Port qualifie l’évidence ; EkoH attribue la réputation ; SmartVote n’utilise que des signaux gouvernés.**
