# Scénarios d’acceptation

## Scénario 1 — Éviter l’effet plafond

Étant donné une personne qui réussit tous les items faciles,  
quand elle passe une épreuve XKaliber,  
alors le système doit augmenter la difficulté,  
et le profil doit indiquer que le niveau initial était maîtrisé mais insuffisant pour mesurer le plafond.

## Scénario 2 — Ne pas humilier une personne sous le niveau attendu

Étant donné une personne qui échoue à un niveau trop difficile,  
quand le système détecte que la difficulté est mal calibrée,  
alors il doit ajuster vers un niveau plus informatif,  
et le rapport doit distinguer échec au niveau supérieur et compétence possible au niveau inférieur.

## Scénario 3 — Produire une certification limitée

Étant donné un profil avec niveau 3 confirmé et niveau 4 partiel,  
quand CertifiKation génère une preuve,  
alors la preuve doit certifier seulement le niveau 3,  
et indiquer que le niveau 4 n’est pas confirmé.

## Scénario 4 — Contester un résultat

Étant donné une personne qui conteste son profil,  
quand elle soumet une demande de révision,  
alors le système doit enregistrer le motif,  
ouvrir une revue humaine,  
et marquer le profil comme contesté jusqu’à décision.

## Scénario 5 — Limiter le signal EkoH

Étant donné un profil XKaliber en analyse de données,  
quand un signal est envoyé vers EkoH,  
alors le signal doit rester borné au domaine concerné,  
et ne doit pas augmenter l’influence de la personne dans des domaines non liés.

## Scénario 6 — Préserver la lecture démocratique

Étant donné un signal de compétence utilisé dans SmartVote,  
quand un résultat de gouvernance est affiché,  
alors la lecture pondérée ne doit pas remplacer la lecture une-personne-un-vote,  
et les règles de pondération doivent être visibles.
