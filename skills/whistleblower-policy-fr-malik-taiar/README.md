# Whistleblower Policy Skill (FR)

Un skill Claude pour **évaluer la conformité** ou **rédiger une politique** de signalement des lanceurs d'alerte conforme au droit français.

## Deux modes d'utilisation

| Mode | Description | Output |
|---|---|---|
| **A. Évaluation de conformité** | Auditer un dispositif existant | Rapport d'évaluation + plan d'actions |
| **B. Rédaction de politique** | Créer un dispositif conforme | Politique complète basée sur le template fourni |

## Cadre juridique couvert

- Directive européenne 2019/1937
- Loi Sapin II modifiée (loi Waserman 2022)
- Décret n°2022-1284
- Référentiel CNIL alertes professionnelles

## Contenu

```
/
├── SKILL.md
├── LICENSE.txt
├── README.md
├── assets/
    ├── Template_Politique_Lanceur_Alerte.docx ← Template pour le Mode B
    ├── [PDF sources]
└── references/
    ├── TEXTES_LEGAUX.md      ← Citations verbatim des articles de loi
    ├── DECRET_PROCEDURE.md   ← Éléments obligatoires (décret 2022-1284)
    ├── RGPD_CNIL.md          ← Conformité RGPD et référentiel CNIL
    ├── FONCTION_PUBLIQUE.md  ← Spécificités fonction publique + art. 40 CPP
    └── VIGILANCE.md          ← Articulation devoir de vigilance
```

## Sources PDF

| Document | Source |
|----------|--------|
| `assets/Directive_2019_1937.pdf` | EUR-Lex |
| `assets/Loi_Sapin_II_consolidee.pdf` | Légifrance |
| `assets/Loi_Waserman_2022.pdf` | Légifrance |
| `assets/Decret_2022_1284.pdf` | Légifrance |
| `assets/Referentiel_CNIL_alertes_professionnelles.pdf` | CNIL |
| `assets/Circulaire_26_juin_2024.pdf` | Circulaires.gouv.fr |
| `assets/DREETS_synthese_2025.pdf` | DREETS |
| `assets/L225-102-1.pdf` et `L225-102-2.pdf` | Légifrance |
| `assets/Directive_CS3D_2024_1760.pdf` | EUR-Lex |

## Utilisation

### Mode A : Évaluation de conformité
1. Collecter les informations (forme juridique, effectif, documentation existante)
2. Appliquer la checklist en 8 phases
3. Produire le rapport (synthèse exécutive, tableau d'évaluation, plan d'actions)

### Mode B : Rédaction de politique
1. Collecter les informations client (canaux, référents, périmètre)
2. Adapter le template `assets/Template_Politique_Lanceur_Alerte.docx` (éléments variables uniquement)
3. Vérifier la conformité avec les références
4. Faire valider par la direction et consulter le CSE

**N'oubliez pas** : Tous les outputs de ce skill doivent être relus par un professionnel du droit qualifié avant toute utilisation à des fins juridiques.

## AVERTISSEMENT

**CECI N'EST PAS UN AVIS JURIDIQUE.** Ce skill est fourni à des fins d'information et d'éducation uniquement. Les lois varient selon les juridictions et les circonstances individuelles, et seul un avocat ou juriste habilité peut fournir un conseil adapté à votre situation spécifique.

## Licence

Voir LICENSE.txt pour les informations de licence.
