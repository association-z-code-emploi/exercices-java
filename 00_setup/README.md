---
tags:
  - exercises
  - java
---

# Setup

Préparons votre environnement de travail pour coder avec Java et effectuer les exercices contenus dans ce dossier "exercices-java" ! Vous aurez d'abord besoin d'un accès au terminal, puis d'installer les outils permettant de compiler et d'exécuter votre code Java.

## Terminal

Selon votre système d'exploitation, vous aurez un terminal différent. L'important n'est pas d'avoir "le meilleur", mais juste d'en avoir un qui puisse exécuter des commandes pour compiler et exécuter votre code.

**Powershell** (Windows), **iTerm2** (macOS) ou **Warp** (Linux) sont par exemple de bons choix.

## Environnement de développement

Ici, vous avez deux options d'installation :

- soit le **Java Developement Kit** (_JDK_) : un ensemble d'outils à installer pour compiler et exécuter du Java dans l'éditeur de code que vous voulez
- soit un **Integrated Developement Environment** (_IDE_) : un logiciel spécifique pour directement coder, débugger et gérer des projets Java plus facilement qu'avec un JDK

> ℹ️ **JDK ou IDE ?**
>
> Ils sont tous les deux fondamentalement différents, mais pour si vous débutez, on peut les différencier ainsi :
>
> - installer le JDK vous permettra de coder sur l'éditeur de votre choix, mais de ne pas oublier de lancer une certaine commande dans le terminal (dont vous aurez de toutes façons besoin) pour compiler votre code
>
> - installer un IDE vous prend en charge les "contraintes" de JDK et vous propose des options pour coder de manière plus agréable ... voire trop : les IDEs sont réputés pour être lourds et pour ralentir votre machine. De plus, tous le monde n'utilise parfois pas le même IDE.

Peu importe votre choix : on indiquera dans ces exercices les deux manières. Néanmoins, suivez attentivement les installations suivantes, sinon relisez-les ou chercher de l'aide en ligne si l'installation ne fonctionne pas correctement.

### JDK

1. Téléchargement :

- allez sur le site [officiel](https://www.oracle.com/java/technologies/downloads) d'Oracle (ou [OpenJDK](https://openjdk.org/) pour sa version OpenSource)
- choisissez la dernière version (ici JDK 23) pour votre système d'exploitation (Windows, macOS, ou Linux)
  - pour Windows : on vous conseillera de télécharger le "**x64 Installer**"
  - pour macOS : on vous conseillera de télécharger le "**x64 DMG Installer**" ou de passer par un gestionnaire d'applicaitons comme [Homebrew](https://formulae.brew.sh/) puis par la formule pour [oracle-jdk](https://formulae.brew.sh/cask/oracle-jdk#default)
  - pour Linux : si vous savez utilisez ce système, vous savez normalement comment télécharger n'importe quel programme ! 😉

2. Installation :

- lancez l'exécutable (par exemple sous Windows, il est recommandé de télécharger "_jdk-23_windows-x64_bin.exe_")
- suivez les instructions jusqu'à compléter l'installation ; notez aussi l'emplacement de l'installation de Java, qui sera utile pour la prochaine étape !

3. Définir les variables d'environnement :

- sous Windows :
  - chercher "_variables d'environnement_" dans votre menu Démarrer
  - dans les "_variables systèmes_" (ou "_variables utilisateur_" si vous avez plus d'une session sur votre ordinateur et qui ne sont pas les vôtres), trouvez la variable "**Path**" et modifiez-la, puis faites "**Nouveau**", puis collez le chemin de l'emplacement où se trouve le dossier "bin" dans le dossier que vous avez installez à l'étape 2 ; probablement "_C:\Program Files\Java\jdk-23\bin_"
- sous macOS/Linux :
  - si vous n'avez pas utilisé un gestionnaire d'applications, ouvez votre terminal et éditez le fichier ".bashrc", ".zshrc" ou ".bash_profile" et ajoutez le code suivant :
    `export JAVA_HOME=/chemin/vers/jdk export PATH=$JAVA_HOME/bin:$PATH` ("/chemin/vers/jdk" devrait être remplacé par l'emplacement où se trouve JDK après téléchargement)

4. Relancez votre ordinateur (ou parfois juste votre terminal)
5. Vérifiez l'installation :

- ouvrez votre terminal et entrez : `java -version` puis appuyez sur la touche "Entrée"
- si Java est correctement intallé, la version devrait s'afficher dans le terminal !

6. Pensez aussi à télécharger un éditeur de code si vous n'en avez encore jamais utilisé : [VSCode](https://code.visualstudio.com/) ou [SublimText](https://www.sublimetext.com/) sont deux valeurs sûres.

### IDE

1. Téléchargement (un seul) :

- [IntelliJ IDEA](https://www.jetbrains.com/idea/) (prenez la "Community Edition" pour la version gratuite ; vous ne perdrez pas grand-chose à la version payante tant que vous êtes débutants)
- [Eclipse](https://www.eclipse.org/)
- [NetBeans](https://netbeans.apache.org/)
- et d'autres que vous avez peut-être rencontré !

2. Installation + suivre les instructions
3. Premier lancement du logiciel ; et c'est tout bon !

## Écrire et exécuter votre premier programme en Java

### JDK

1. Dans un dossier "exercices-java", puis dans le sous-dossier "00_setup", créez un fichier "HelloWorld.java"

```txt
📂 exercices-java
│── 📂 00_setup
    │── 📝 HelloWorld.java
    │── 📝 README.md (le fichier que vous êtes actuellement en train de lire 👋)
```

2. Dans votre éditeur de code, écrivez le code suivant dans le fichier "HelloWorld.java" :

```java
class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello, you magnificent beast!");
  }
}
```

3. Dans votre terminal, allez à l'emplacement de votre dossier "00_setup" (par exemple, avec PowerShell, faites `cd <le path du dossier>`) puis entrez la commande `javac HelloWorld.java` : un nouveau fichier va être créé dans le dossier "00_setup", et qui devrait se nommer "HelloWorld.class"
4. À partir de là, il ne vous reste plus qu'à entrez la commande `java HelloWorld` pour voir le résultat de votre code. Ici, vous devriez lire la phrase "Hello, you magnificent beast!". 👏

> ℹ️ **_"Pourquoi le fichier généré se nomme HelloWorld.class ?"_**
>
> La nomenclature des fichiers et des classes est très stricte en Java : le nom d'un fichier ".class" (et on conseille d'en faire autant avec un fichier ".java") DOIT prendre le nom de la classe dans le fichier ".java".
>
> Ici, le code de l'étape 2 a un nom de class "HelloWorld" et malgré que le nom de son fichier soit "HelloWorld.java", le fichier généré sera "HelloWorld.class".

### IDE

1. Créez un nouveau projet Java (_Java Project_)
2. Créez une nouvelle classe Java ("_Java Class_")
3. Ajoutez le code suivant dans votre fichier ".java" :

```java
class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello, you magnificent beast!");
  }
}
```

4. Cliquez sur le bouton "Run" ou "Execute" et la console devrait s'ouvrir avec le résultat : "Hello, you magnificent beast!" 👏
