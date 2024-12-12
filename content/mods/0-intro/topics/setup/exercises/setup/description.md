# Instructions d'installation des outils

Dans ce fichier, vous trouverez des instructions pour installer les outils que nous utiliserons pendant le cours.

Tous ces outils sont disponibles pour les utilisateurs de Linux, macOS et Windows.
Nous aurons besoin de ces outils pour écrire et compiler notre code Rust, ainsi que pour permettre le mentorat à distance.  
*Important : ces instructions doivent être suivies à la maison avant le début du premier tutoriel.*  
*Si vous rencontrez des problèmes lors de l'installation, contactez les enseignants ! Nous ne traiterons pas les problèmes d'installation pendant le premier tutoriel.*

## Rust et Cargo
Nous aurons tout d'abord besoin de `rustc`, le compilateur Rust standard.  
`rustc` est généralement utilisé via `cargo`, le gestionnaire de packages de Rust.  
`rustup` s'occupe d'installer `rustc` et `cargo`.

Cette étape est simple : rendez-vous sur <https://rustup.rs> et suivez les instructions.  
Assurez-vous d'installer la dernière version de la toolchain par défaut. Une fois terminé, exécutez :

```bash
rustc -V && cargo -V
```

Vous devriez obtenir une sortie similaire à ceci :

```bash
rustc 1.67.1 (d5a82bbd2 2023-02-07)
cargo 1.67.1 (8ecd4f20a 2023-01-10)
```

Avec Rustup, vous pouvez installer des toolchains et des composants Rust. Plus d'infos :  
- <https://rust-lang.github.io/rustup>
- <https://doc.rust-lang.org/cargo>

## Rustfmt et Clippy
Pour éviter les discussions, Rust fournit son propre outil de formatage : Rustfmt.  
Nous utiliserons également Clippy, une collection de lints qui analyse votre code et détecte des erreurs courantes. Vous verrez que Clippy peut être un compagnon très utile.  
Rustup installe Rustfmt et Clippy par défaut.

Pour exécuter Rustfmt sur votre projet, lancez :

```bash
cargo fmt
```

Pour exécuter Clippy :

```bash
cargo clippy
```

Plus d'infos :  
- Rustfmt : <https://github.com/rust-lang/rustfmt>  
- Clippy : <https://github.com/rust-lang/rust-clippy>  

## Visual Studio Code
Pendant le cours, nous utiliserons Visual Studio Code (vscode) pour écrire du code.  
Bien sûr, vous êtes libre d'utiliser votre éditeur préféré, mais en cas de problème, nous ne pourrons pas vous assister.  
Nous utiliserons également vscode pour permettre la collaboration et le mentorat à distance pendant les sessions tutorées.

Les instructions d'installation se trouvent ici : <https://code.visualstudio.com/>.

Nous installerons également quelques plugins.  
Le premier est Rust-Analyzer. Les instructions d'installation se trouvent ici : <https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer>.  
Rust-Analyzer fournit une aide précieuse pendant le développement et est indispensable pour débuter avec Rust.

Un autre plugin que nous installerons est Live Share.  
Nous utiliserons ce plugin pour partager nos écrans et fournir de l'aide pendant les sessions tutorées à distance.  
Le pack d'extensions contient également Live Share Audio, qui permet une communication audio pendant les sessions partagées.  
Les instructions d'installation sont disponibles ici : <https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare>.  

Enfin, nous utiliserons le plugin CodeLLDB, qui permet le débogage du code Rust directement depuis vscode.  
Les instructions d'installation sont ici : <https://marketplace.visualstudio.com/items?itemName=vadimcn.vscode-lldb>.  

Plus d'infos :  
- <https://rust-analyzer.github.io/>  
- <https://code.visualstudio.com/learn/collaboration/live-share>  

## Git
Nous utiliserons Git comme outil de gestion de versions.  
Si vous ne l'avez pas encore installé, vous trouverez des instructions ici : <https://git-scm.com/book/en/v2/Getting-Started-Installing-Git>.  
Si vous débutez avec Git, vous apprécierez également l'introduction proposée par GitHub : <https://docs.github.com/en/get-started/using-git/about-git>.  
Vous pouvez aussi consulter l'introduction à Git avec vscode : <https://www.youtube.com/watch?v=i_23KUAEtUM>.  

Plus d'infos : <https://www.youtube.com/playlist?list=PLg7s6cbtAD15G8lNyoaYDuKZSKyJrgwB->  

## Code du cours
Une fois tout installé, vous pouvez cloner le dépôt de code source.  
Le dépôt se trouve ici : <https://github.com/tweedegolf/teach-rs>.  

Les instructions pour cloner le dépôt sont disponibles ici : <https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls>.  

# Testez votre configuration
Une fois le code téléchargé sur votre machine, accédez-y depuis votre terminal favori et exécutez :

```
cd #[modmod:exercise_dir]
cargo run
```

La première exécution peut prendre un moment, car Cargo va récupérer l'index des crates depuis le registre.  
Il compilera et exécutera le package `intro`, que vous trouverez dans `#[modmod:exercise_dir]`.  
Si tout se passe bien, vous devriez voir une sortie semblable à ceci :

```
   Compiling intro v0.1.0 ([REDACTED]/#[modmod:exercise_dir])
    Finished dev [unoptimized + debuginfo] target(s) in 0.11s
     Running `target/debug/intro`
🦀 Hello, world! 🦀
Vous avez réussi à compiler et exécuter votre premier projet Rust !
```

Si Rust-Analyzer est correctement configuré, vous pouvez également cliquer sur le bouton "▶️ Run" qui apparaît dans `#[modmod:exercise_dir]/src/main.rs`.  
Avec CodeLLDB installé, vous pouvez démarrer une session de débogage en cliquant sur "Debug", juste à côté du bouton "▶️ Run".  
Amusez-vous à définir des points d'arrêt en cliquant sur un numéro de ligne (un cercle rouge apparaîtra) et en utilisant les contrôles pour avancer pas à pas dans le code.  
Vous pouvez voir les valeurs des variables en survolant leur nom lorsque l'exécution est en pause, ou en explorant la vue "Local" sous "Variables" dans le panneau gauche pendant une session de débogage.
