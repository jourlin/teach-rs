Compagnon de l'enseignant pour teach-rs
=======================================

Si vous avez décidé d'essayer teach-rs pour vos étudiants, vous rencontrerez probablement deux problèmes :

1. En tant qu'académique, vous pourriez estimer que vos connaissances pratiques de Rust sont insuffisantes.

2. Vous devrez sélectionner les sujets pour respecter des contraintes pratiques.

Quels éléments de teach-rs devriez-vous enseigner à vos étudiants ? Et combien de temps cela prendra-t-il ?

Nous supposons que vous avez une idée claire de vos objectifs pédagogiques et de votre public cible. Teach-rs peut être utilisé pour des étudiants de première année à l'université, des étudiants en master, ou même pour une formation interne destinée à des ingénieurs confirmés dans votre entreprise de logiciels, mais évidemment, chaque groupe nécessitera une approche différente !

Teach-rs est un cours modulaire
===============================
Nous avons défini des *pistes* spécifiques, qui consistent en des sélections de modules cohérents en fonction d'un objectif d'apprentissage et d'un public cible. Par exemple, teach-rs orienté sur la programmation Web ou teach-rs orienté sur les appareils embarqués. Vous pouvez consulter la liste complète des pistes [ici](./README.md#pre-defined-tracks) :

Modularité plus fine
--------------------
Si vous souhaitez un contrôle plus précis sur la sélection du contenu, chaque module est structuré en plusieurs *sujets*. Un sujet est défini par un ensemble de diapositives et des exercices recommandés. Vous pouvez construire vos propres modules en sélectionnant des sujets. Nous avons défini des dépendances entre les sujets ; par exemple, si vous choisissez le sujet `basic-syntax`, vous devriez également inclure le sujet `why-rust`. Ces dépendances garantissent que votre cours reste cohérent.

Cependant, si vous empruntez cette voie, vous devrez vous assurer vous-même que la charge de travail reste équilibrée, car, contrairement aux modules, les *sujets* n'ont pas de temps d'étude fixe associé. Par exemple, le sujet `why-rust` demandera moins de temps (et n'inclut aucun exercice pratique) que le sujet `basic-syntax`. Comme teach-rs est en développement actif, nous ne pouvons pas fournir d'estimations de temps par sujet et nous nous concentrons davantage sur l'équilibrage de la charge de travail pour le cours complet et les *pistes* prédéfinies.

Aperçu des modules et des sujets
--------------------------------
Les modules généraux du cours Rust peuvent être divisés en modules "communs" et "spécialisés". Les modules communs seront utiles pour toutes les pistes (par exemple, "Bases du langage"), tandis que d'autres peuvent être considérés comme optionnels (par exemple, "Rust pour le Web").

Le module 0 (introduction) est recommandé dans son intégralité pour tous les cours, car il explique les motivations pour apprendre Rust et présente globalement ses fonctionnalités. Le module A contient tous les sujets liés aux fonctionnalités du langage.

Matériel de référence
=====================
Plusieurs ressources en ligne sont disponibles pour fournir un précieux matériel de référence pour vous (ou vos étudiants).

- [The Rust Programming Language](https://doc.rust-lang.org/book/index.html), un livre en ligne, également disponible [en version papier](https://nostarch.com/rust-programming-language-2nd-edition).
- [Rust by Example](https://doc.rust-lang.org/stable/rust-by-example/), une référence en ligne avec des exemples idiomatiques de code Rust.
- [Rust for Rustaceans](https://nostarch.com/rust-rustaceans), un livre qui suppose une connaissance préalable et aborde des sujets plus avancés.
- [Learning Rust with Entirely Too Many Linked Lists](https://rust-unofficial.github.io/too-many-lists/), axé sur les règles de possession et d'emprunt de Rust.
- [Rust Design Patterns](https://rust-unofficial.github.io/patterns/), une collection de modèles idiomatiques Rust (et d'anti-modèles).
- [The Rust Reference](https://doc.rust-lang.org/reference/index.html), une référence pour trouver des explications sur des points plus fins de syntaxe et de sémantique.
- [The Rustonomicon](https://doc.rust-lang.org/nomicon/), une référence spécifique aux aspects bas niveau, interfaces binaires d'application et au code `unsafe`.

Solutions des exercices
-----------------------
Teach-rs est fourni sans réponses aux exercices. Si vous avez besoin de ces réponses, veuillez [nous contacter](mailto:hd@oordt.dev).
