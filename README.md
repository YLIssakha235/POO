### C#
le C# : est un langage de programmation développé par Microsoft pour le developpement d'application Windows. Il utilise le farmework DOTnet. Ce qui nous permet de developper dans le WEB, MOBILE ...

---

### Objet
un objet est une variable qui possède deux types de membres 
- des attributs (caractéristiques)
- des methodes (fonctionnalités)

---

### Classes 
- une classe est une maquette qui permet la construction des objets
- un objet est une instance d'une classe. on crée un objet à partir d'une classe.
- pour créer un nouvel objet on utilise le mot new suivi de la classe
- exemple : Contact lur = new Contact ("Question", "Lurkin")

---

### instances
Une instance est un ensemble de :
- une classe est un modèle
- un objet est une instance d'une classe.
- une variable stocke une référence vers l'objet

---

### Alias 
On sait q'une variable est une référence vers un objet. la variable permet d'accéder à l'objet et ainsi le manipuler. 
- un alias référe le meme objet q'une varibale
- on peut donc avoir 2 variables qui pointent vers le meme objet

---

### Définir une classe 
Dans une classe, on définit la liste des méthodes
- le constructeur initialise l'etat de l'objet.
- initialisation des variables d'instance

---

### Vie d'un objet 
Trois étapes principales dans la vie d'un objet 
- création de l'objet (initialisation)
- appel de méthode et changement d'etat (utilisation)
- Destruction de l'objet (finalisation) : c'est à dire quand aucune varialbe est liée à lui.
  
  
---
### Variable d'instance 
- une variable d'instance est liée à l'objet car sa valeur fait partie de l'etat de l'objet.
- Peuvent avoir une certaine visibilité, uniquement accessible dans la classe ou visible de l'exterieur.

---

### instanciation
c'est le fait de créer plusieurs instances d'une classe. Chaque instance a son identité propre.

---

### Méthodes
- Une méthode (d'instance) représente une fonctionnalité. Elle agit sur une instance spécifique, l'objet cible.
- Mot réservé spécifique pour acceder à l'objet, réference vers l'objet cible. on utilise (this).
- Peuvent avoir une certaine visibilité, uniquement dans la classe ou visible de l'exterieur.

---

### Surchage de méthode 
- plusieurs méthodes peuvent avoir le meme nom, meme si les types de la liste de différe.

---

### Résolution de la surcharge 
- construction liste des types des paramètres réels
- identification des methodes accessibles avec le type statique
- recherche d'une méthode avec la meme liste de types
- recherche des methodes avec parametre compatibles
- choix de la methode la plus spécifique


---
### Aggrégation 
Est une rélation entre deux classe ou une classe ("contenante") contient une reference à une ou plusieurs instances d'une autre classe ('la classe contenue"). Mais leur cycle de vie est indépendant.

---

### Couplage et cohésion
- classes couplées si l'un dépend de l'implémentation de l'autre
    - une claasse accède aux variables d'instance de l'autre
      
- cohésion d'une classe mesure son niveau d'independacne
    - classe cohérente facilement maintenable et réutilisable.

- il faut minimiser (réduire) le couplage et maximiser (augmenter) la cohésion
    - Regle de bonne pratique en POO
    - on plus on est couplé au moins on a de la cohésion.

---

### Visibilité
la visibilité fait référence au niveau d'accès ou à la portée des membres (champs, propriètés, méthodes ...) ou des classes dans le code. Elle determine quelles parties du programme peuvent accéder à ces memebres ou classes.

- Visibilité public : accessible de partoutn dans toutes les classes et assemblages
- visibilité private : accessible uniquement dans la classe ou il est défini
    - c'est le niveau de visibilité par défaut.
- Protected : accessible dans la classe ou il est defini et dans toutes les classes dérivées.
- interne : accessible uniquement dans le même assemblage ( fichier de compilation)

---

### Bonnes pratiques
Restez minimaliste, utilisez private par defaut et exposez uniquement ce qui est strictement nécessaire pour garantir la sécurité et la maintenabilité du code.

---

### Encapsulation 
l'encapsulation est un principe fondamental de POO qui consiste à regrouper des données (champs) et des méthodes dans une classe, tout en controlant leur accès à l'aide de niveaux de visibilité.
- elle permet de cacher les détails d'implémentaiton d'une classe tout en exposant une interface controlée.

---

### Avantages
- les données sensibles sont protégées
- l'accès est controlé via des interfaces claires et fiables
- les détails internes restent cachés, ce qui améliore la maintenabilité et la sécurité du code.
  
---

### Interface publique
Elle sert à standardiser les comportements des classes tout en favorisant l'abstraction et le polymorphisme.


---

### Immuabilité
l'immuabilité signifie qu'un objet ne peut pas etre modifier apres sa creation. Toute tentative de modification crée un nouvel objet au lieu de changer l'objet existant.

- les avantages:
    - evite les erreurs liées aux modifications
    - favorise la sécurité des threads
    - simplifie le débogage et la maintenace.

---

### Héritage
l'heritage est un mecanisme qui permet à une classe (dérivée) de reutiliser et etender les fonctionnalités d'une autre classe (classe de base).

- Reutilisation du code
- extensibilité: ajouter de nouvelles fonctionnalités dans les classes dérivées
- organistaion : structure clare grace aux relations entre les classes.

---

### Polymorphisme 
le polymorphisme est la capacité d'une methode, d'une classe ou d'un objet à prendre plusieurs formes. il permet d'utiliser une meme interface ou methode pour des comportements differents.


---

### Type statique vs Dynamique
- Type statique
    - defini au moment de la compilation
    - le type de variable ne change pas et doit etre declare explicitement
    - les erreurs liées aux types sont detectées à la compilaiton
    - (+) meilleure sécurité
    - (+) améliore les performances
    - (+) aide à detecter les erreurs tot
      
- Type dynamique
    - defini au moment de l'execution
    - le type peut changer et aucune verif n'est effectue  à la compilation
    - (+) plus flexible
    - (+) utilise pour travailler avec des API

on utilise les types statiques pour la sécurité et la performance, et les types dynamiques uniquement lorsque c'est necessaire.

---

###



