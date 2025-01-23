### **C#**
Le **C#** est un langage de programmation développé par Microsoft pour le développement d'application Windows. Il utilise le framework **.NET**, ce qui permet de développer pour le **web**, le **mobile**, etc.

---

### **Objet**
Un **objet** est une variable qui possède deux types de membres :  
- des **attributs** (caractéristiques)  
- des **méthodes** (fonctionnalités)  

---

### **Classes**
- Une **classe** est une maquette qui permet la construction des objets.  
- Un **objet** est une instance d'une classe. On crée un objet à partir d'une classe.  
- Pour créer un nouvel objet, on utilise le mot-clé **`new`** suivi de la classe.  
- Exemple : `Contact lur = new Contact("Question", "Lurkin");`

---

### **Instances**
Une **instance** est un ensemble de :  
- Une classe (modèle).  
- Un objet (instance d'une classe).  
- Une variable qui stocke une référence vers l'objet.  

---

### **Alias**
On sait qu'une variable est une référence vers un objet. La variable permet d'accéder à l'objet et de le manipuler.  
- Un **alias** réfère le **même objet** qu'une variable.  
- Il est possible d'avoir **deux variables** qui pointent vers le même objet.  

---

### **Définir une classe**
Dans une **classe**, on définit :  
- Une **liste des méthodes**.  
- Le **constructeur** pour initialiser l'état de l'objet.  
- L'initialisation des **variables d'instance**.  

---

### **Vie d'un objet**
Trois étapes principales dans la vie d’un objet :  
1. **Création** de l’objet (initialisation).  
2. **Utilisation** (appel de méthode et changement d’état).  
3. **Destruction** de l’objet (finalisation).  

---

### **Variable d’instance**
- Une **variable d’instance** est liée à l’objet.  
- Elle peut avoir une visibilité : accessible uniquement dans la classe ou visible depuis l’extérieur.  

---

### **Instanciation**
L’**instanciation** consiste à créer plusieurs instances d'une classe. Chaque instance a sa propre identité.  

---

### **Méthodes**
- Une **méthode d’instance** représente une fonctionnalité.  
- Elle agit sur une instance spécifique (objet cible).  
- On utilise le mot-clé **`this`** pour accéder à l’objet cible.  
- Elles peuvent avoir une visibilité spécifique.  

---

### **Surcharge de méthode**
- Plusieurs méthodes peuvent avoir le même nom, mais avec des **listes de paramètres différents**.

---

### **Résolution de surcharge**
1. Construction de la **liste des types des paramètres réels**.  
2. Identification des **méthodes accessibles** via le type statique.  
3. Recherche d’une méthode avec une **liste de types exacte**.  
4. Recherche des méthodes avec des **paramètres compatibles**.  
5. Choix de la méthode la **plus spécifique**.  

---

### **Agrégation**
Une **agrégation** est une relation entre deux classes où :  
- Une classe "contenante" contient une référence à une ou plusieurs instances d'une autre classe ("contenue").  
- Leur cycle de vie est indépendant.  

---

### **Couplage et cohésion**
- **Couplage** : Classes couplées si l'une dépend de l'implémentation de l'autre.  
- **Cohésion** : Mesure de l’indépendance d’une classe.  
  - Classes cohérentes = Facilement maintenables et réutilisables.  
- **Bonnes pratiques** :  
  - Minimiser le **couplage**.  
  - Maximiser la **cohésion**.  

---

### **Visibilité**
- la visibilité determine quelles parties du programme peuvenet accéder à ces membres ou classes.
- **Public** : Accessible partout.  
- **Private** : Accessible uniquement dans la classe.  
- **Protected** : Accessible dans la classe et ses dérivées.  
- **Interne** : Accessible dans le même assemblage.  

---

### **Bonnes pratiques**
Utilisez **private** par défaut et exposez uniquement ce qui est nécessaire pour la sécurité et la maintenabilité.  

---

### **Encapsulation**
- **Encapsulation** : Regrouper les données et méthodes dans une classe en contrôlant leur accès.
- comment cela fonctionne :
  - 1) **visibilité**: utilisation de private, protected, public
  - 2) **Methodes d'acces** : utilise (getters/setters), permettant de lire ou modifier les données de manière securisée.
        
- Avantages :  
  - Cacher les détails d'implémentation.  
  - Exposer une interface contrôlée.  

---

### **Avantages**
- Protection des données sensibles.  
- Accès contrôlé via des interfaces claires.  
- Amélioration de la maintenabilité et de la sécurité du code.  

---

### **Interface publique**
Une interface publique standardise les comportements des classes et favorise l’abstraction et le polymorphisme.  

---

### **Immuabilité**
Un objet **immutable** ne peut pas être modifié après sa création.  
- **Avantages** :  
  - Évite les erreurs.  
  - Favorise la sécurité des threads.  
  - Simplifie le débogage.  

---

### **Héritage**
L’**héritage** permet :  
- La réutilisation du code.  
- L’extensibilité des classes dérivées.
- est un mecanisme qui permet à une classe (dérivée) de reutiliser les fonctionnalités d'une autre classe (classe base). 

---

### **Polymorphisme**
Le **polymorphisme** permet à une méthode, une classe ou un objet de prendre plusieurs formes via une interface commune.  

---

### **Types statiques vs dynamiques**
- **Statique** : Défini à la compilation. Le type de variable ne change pas.
- (+) meilleur sécurité; améliore les performances; aide à detecter les erreurs tot. 
- **Dynamique** : Défini à l’exécution. Le type peut changer.
- (+) plus flexible; utiliser pour travailler avec des API
- Utilisez les types statiques pour la sécurité et les performances.  

---

### **Interfaces**
Une **interface** est une structure qui impose un comportement standardisé.  
- Favorise l’abstraction et le polymorphisme.  

---

### **Classes abstraites**
- Est une base ou modèle pour d'autres classes.
- Fournissent un modèle commun.  
- Forcent les classes dérivées à implémenter certaines méthodes.
- Les classes abstraites soutiennent principalement:
    - OCP (Open/Closed Principale) : une classe doit etre ouverte à l'extention mais ferme à la modification.
    - LSP ( Liskov Substitution Principale) : les objets d'une classe dérivée doivent pourvoir remplacer les objets de base sans alterer le comportement du programme.

---

### Implementation override
- le mot-clé override est utilisé pour rédefinir une methode virtuelle ou abstraite dans une classe dérivée, permettant d'adapter ou d'etendre le comportemnet d'une classe de base.
- Virtual : la methode a deja une implémentation, mais peut etre modifiée dans les classes dérivées.
- abstrait : la méthode n'a pas d'implementation et doit etre definie dans les classes dérivées.

---

### **Principe SOLID**
- **S** : Une responsabilité par classe. ( *Single Responsibility Principe*)
    - les classes et les methodes ne doivent etre responsables que d'une chose.
    - Cela permet d'avoir une grande cohésion.
- **O** : Ouvert à l’extension, fermé à la modification. (*Open/Closed Principal*)
    - open : le code doit etre ouvert aux extensions
    - closed : le code doit etre fermé aux modifications.
- **L** : Classe dérivée remplaçable. (*Liskov Substitution Principale*)
    - une classe derivée peut remplacer sa classe de base.
- **I** : Interfaces spécifiques. (*Interface Segregation Principale*)
- **D** : Dépendre des abstractions. (*Dependecy Inversion Principale*)
  

---

### **STUPID**
les principes STUPID representent des antipatterns en developpement logiciel, c'est à dire des pratiques à eviter. Ces principes sont l'opposé des principes SOLID et conduisent à un code difficile ) maintenir, tester et comprendre.
Les antipatterns **STUPID** sont à éviter :  
- **S** : Singleton abusif.(*Singleton: rendant le code rigide et difficile à tester*)
- **T** : Couplage fort.(*Tight Coupling: limite la flexibilité*)
- **U** : Code difficile à tester.(*Untestabillity : du à un mauvais design*)  
- **P** : Optimisation prématurée.(*Optimisation inutile qui complique le code*)  
- **I** : Noms peu descriptifs.(*Indescriptive Naming: Noms non clairs, rendant le code difficle à comprendre*)
- **D** : Code dupliqué. (*Repetition de code, augmentant les risques de bugs*)

Eviter les pratiques STUPID permet de creer un code clair, modulaire et maintenanble, ce qui est renforcé par l'application des principes SOLID.

---

### **Modélisation UML**
La **modélisation UML** est un outil visuel pour concevoir et documenter des systèmes logiciels. elle utilise des diagrammes variés pour representer la structure et le comportement d'un systeme ce qui est efficace pour un developpement organisé.

- Clarité.
- standarisation
- Communication.  
- Réduction des erreurs.

---

### Patterns
- Servent à resoudre des problèmes récurrents et à rendre le code modulaire, flexible, reutilisable et maintenable.
- Pattern de création :
    - singleton : garantit une seule instance d'une classe
    - Factory Method : crée des objets sans les exposer
    - Abstract Factory: Crée des familles compatibles
    - Builder : construit des objets complexes étape par étape.
- Pattern Structurels:
    - Adapter : rend compatibles deux interfaces
    - Bridge : sépare abstraction et implémentaiton
    - Composite : Traite des groupes d'objets comme un seul
    - Decorator : Ajoute des fonctionnalités sans modifier la structure.
- Patterns comportementaux:
    - Oberser : met à jour les objets dependants
    - Strategy : permet de changer l'algorithme dynamiquement.
    - State : modifie le comportement d'un objet selon son état
    - command: encapsule une requete pour une execution flexible
- Patterns Architectiraux :
    - MVC : sepate donnees, interface, et logique utilisateur.
    - MVVM : Simplifie le lien entre interface et logique.
    - Layered Architecture : organise en couches (ex: presentation, logique, donnees)
    - event-Driven: base sur des declenchements d'evenements.
    - 
