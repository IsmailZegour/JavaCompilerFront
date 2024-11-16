
# **Java Online Compiler - Frontend**

## **Description**

Java Online Compiler est une application web moderne qui offre une interface fluide pour écrire, compiler et exécuter du code Java directement dans votre navigateur. Construit avec **Angular**, le frontend propose un design élégant et intuitif, propulsé par **Monaco Editor** pour une expérience de codage supérieure.

Ce projet communique avec une API backend pour gérer la compilation et l'exécution du code, ce qui en fait un outil parfait pour les développeurs, les étudiants et toute personne apprenant Java.

---

## **Fonctionnalités**

- 🖋 **Éditeur de code intégré** : Propulsé par Monaco Editor pour la coloration syntaxique et la détection d'erreurs.
- ⚡ **Exécution du code en temps réel** : Compilez et exécutez du code Java instantanément.
- 📜 **Affichage des résultats** : Visualisez la sortie d'exécution dans un panneau dédié.
- 📱 **Design réactif** : Fonctionne parfaitement sur tous les appareils et tailles d'écran.

---

## **Prérequis**

Pour exécuter ce projet localement, assurez-vous d'avoir les éléments suivants installés :

- **Node.js** (v16 ou supérieur)
- **Angular CLI** (v15 ou supérieur)

---

## **Installation et Configuration**

1. **Clonez le dépôt** :
   ```bash
   git clone https://github.com/votre-utilisateur/java-online-compiler-frontend.git
   cd java-online-compiler-frontend
   ```

2. **Installez les dépendances** :
   ```bash
   npm install
   ```

3. **Démarrez le serveur de développement** :
   ```bash
   ng serve
   ```

4. **Accédez à l'application** :
   Ouvrez votre navigateur et naviguez vers :
   ```
   http://localhost:4200
   ```

---

## **Comment Utiliser**

1. Écrivez votre code Java dans l'éditeur intégré.
2. Cliquez sur le bouton **Run Code** pour envoyer votre code au backend pour compilation et exécution.
3. Visualisez le résultat dans le panneau d'affichage situé sous l'éditeur.

---

## **Intégration de l'API**

Le frontend communique avec l'API backend, hébergée à `http://localhost:8080`.

### **Exemple de Requête et Réponse de l'API**

- **POST /compile**
  - **Corps de la requête** :
    ```json
    {
      "code": "public class Main { public static void main(String[] args) { System.out.println(\"Hello, World!\"); }}"
    }
    ```
  - **Réponse** :
    ```json
    {
      "output": "Hello, World!"
    }
    ```

---

## **Structure du Projet**

```
src/
├── app/
│   ├── code-editor/       # Composant pour l'écriture et l'exécution du code
│   ├── shared/            # Utilitaires et services partagés
│   └── assets/            # Assets statiques
├── environments/          # Configurations spécifiques à l'environnement
```

---

## **Technologies Utilisées**

- **Angular** : Framework pour construire le frontend.
- **Monaco Editor** : Éditeur de code riche avec coloration syntaxique.
- **RxJS** : Bibliothèque de programmation réactive pour gérer les flux de données asynchrones.

---

## **Problèmes Connus**

- Assurez-vous que le serveur backend est en cours d'exécution et correctement configuré pour **CORS** afin d'éviter les problèmes de connexion.

---

## **Contributions**

Les contributions sont les bienvenues ! Si vous souhaitez contribuer :

1. **Forkez le dépôt**.
2. **Créez une branche pour votre fonctionnalité**.
3. **Soumettez une pull request** avec des modifications détaillées.

---

## **Licence**

Ce projet est sous licence **MIT License**. Consultez le fichier LICENSE pour plus de détails.

---

🚀 Commencez à coder en Java directement dans votre navigateur avec **Java Online Compiler** dès aujourd'hui !
