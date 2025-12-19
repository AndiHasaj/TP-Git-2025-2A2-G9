## Reflexion

1. **Structure du projet Git :**
   - Branches principales : `branch/Senard` (moi), `branch/ahasaj` (Élève 1), `branch/fgrolleau` (Élève 3)
   - J’ai créé mes fichiers `tp.md` et `reflexion.md` sur ma branche, puis mergé la branche d’Élève 3 avec fast-forward.
   - J’ai reverté le commit `index.html` d’Élève 1 sur ma branche.
   - Exemple graphique de l’historique :
     ```
     * f694fb6 (HEAD -> branch/Senard) merge/Senard: merge de branch/fgrolleau
     * ffcd6f4 feat/Senard: ajout de tp.md et reflexion.md
     * 508c8e2 feat/ahasaj : création d'index.html
     * 0a73267 Instructions TP Final
     * ...
     ```

2. **Différence `git fetch` / `git pull` :**
   - `git fetch` récupère les commits distants mais **ne modifie pas ma branche locale**.
   - `git pull` récupère et merge automatiquement les commits dans ma branche locale.
   - Exemple concret : j’ai utilisé `git fetch` pour vérifier les branches d’Élève 1 et 3 avant de les merger.

3. **Différence `git reset` / `git revert` :**
   - `git reset` supprime des commits de l’historique (risqué si la branche est partagée).
   - `git revert` crée un commit qui **annule un commit existant** sans toucher à l’historique.
   - Exemple concret : j’ai utilisé `git revert` pour annuler le commit `index.html` d’Élève 1 sur ma branche.
