# Académie des Sorciers — TypeScript

Projet **TypeScript** (Node.js) qui met en pratique des notions clés du langage à travers un mini-domaine “Académie des sorciers” : gestion de sorciers, sorts, événements typés, décorateurs et *type guards*.

## Fonctionnalités (exercices couverts)

1. **Gestion des sorciers** — ajout et consultation via un dépôt générique.
2. **Filtrage par maison** — recherche des sorciers par `House` (`Gryffindor`, `Slytherin`, `Ravenclaw`, `Hufflepuff`).
3. **Événements typés** — union discriminée `AcademyEvent` et extraction de `SpellCastEvent` avec `Extract`.
4. **Validation par décorateur** — `@ValidateSpellPower` refuse une puissance de sort négative.
5. **Cache de méthode** — `@Cache` mémorise les résultats par instance/arguments.
6. **Type Guards** — `isHouse` / `isWizard` pour valider des données `unknown` à l’exécution.

## Prérequis

- [Node.js](https://nodejs.org/) (recommandé : version LTS récente)

## Installation

```bash
npm install
```

## Utilisation

```bash
# Exécuter la démonstration (ts-node)
npm start

# Vérifier la compilation TypeScript
npm run build
```

La sortie compilée est générée dans `dist/` (selon `tsconfig.json`).

## Structure du projet

```text
.
├── src/
│   ├── types.ts         # Types et interfaces (Wizard, Spell, AcademyEvent, ...)
│   ├── repository.ts    # GenericRepository, WizardRepository, SpellRepository
│   ├── decorators.ts    # @ValidateSpellPower, @Cache
│   └── main.ts          # Scénarios de démonstration des exercices
├── package.json
├── tsconfig.json
└── README.md
```

## Technologies

- **TypeScript** (`strict`, `experimentalDecorators`)
- **ts-node** pour l’exécution en développement
- Cible **ES2020**, module **CommonJS**

## Licence

Projet personnel / éducatif.
