# Frontières de données

## Séparer les couches

XKaliber doit séparer clairement les objets suivants :

1. **Données de session** : réponses, temps, items, progression.
2. **Interprétation** : niveau estimé, confiance, erreurs typiques.
3. **Profil** : version lisible et partageable du résultat.
4. **Preuve CertifiKation** : attestation minimale et vérifiable.
5. **Paquet d’évidence K-Port** : preuve source, bornée par domaine, avec provenance, statut, validité, confiance et consentement.
6. **Signal EkoH** : signal de scoring préparé par K-Port à partir de l’évidence admissible.
7. **Décision externe** : embauche, accès, promotion ou participation.

## Raison

Une même évaluation peut servir à plusieurs usages, mais chaque usage doit avoir sa propre limite.

Exemple :

- une école peut voir le détail pédagogique ;
- une organisation peut voir le niveau certifié ;
- K-Port peut recevoir un paquet d’évidence source vérifiable ;
- EkoH peut recevoir de K-Port un signal de scoring borné par domaine ;
- SmartVote ne devrait jamais recevoir les réponses brutes ni un signal direct de XKaliber ;
- un public ne devrait pas voir le profil sans consentement.

## Principe

**Plus l’usage est éloigné de l’évaluation initiale, plus le signal doit être résumé, contextualisé et limité.**

La frontière d’autorité est également explicite : **XKaliber mesure, CertifiKation atteste, K-Port qualifie et route l’évidence, EkoH calcule la réputation.**
