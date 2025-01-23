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

---

### **Polymorphisme**
Le **polymorphisme** permet à une méthode, une classe ou un objet de prendre plusieurs formes via une interface commune.  

---

### **Types statiques vs dynamiques**
- **Statique** : Défini à la compilation.  
- **Dynamique** : Défini à l’exécution.  
- Utilisez les types statiques pour la sécurité et les performances.  

---

### **Interfaces**
Une **interface** impose un comportement standardisé.  
- Favorise l’abstraction et le polymorphisme.  

---

### **Classes abstraites**
- Fournissent un modèle commun.  
- Forcent les classes dérivées à implémenter certaines méthodes.  

---

### **Principe SOLID**
- **S** : Une responsabilité par classe.  
- **O** : Ouvert à l’extension, fermé à la modification.  
- **L** : Classe dérivée remplaçable.  
- **I** : Interfaces spécifiques.  
- **D** : Dépendre des abstractions.  

---

### **STUPID**
Les antipatterns **STUPID** sont à éviter :  
- **S** : Singleton abusif.  
- **T** : Couplage fort.  
- **U** : Code difficile à tester.  
- **P** : Optimisation prématurée.  
- **I** : Noms peu descriptifs.  
- **D** : Code dupliqué.  

---

### **Modélisation UML**
La **modélisation UML** est un outil visuel pour concevoir et documenter des systèmes logiciels.  
- Clarité.  
- Communication.  
- Réduction des erreurs.  
