# DevTasks


Aplicació web senzilla de gestió de tasques desenvolupada amb HTML, CSS i JavaScript, utilitzada com a projecte base per a una pràctica integral de DevOps i Integració Contínua (CI/CD) amb GitHub.

## Funcionalitats
- Crear tasques
- Completar tasques
- Eliminar tasques
- Filtrar tasques
- Veure estadístiques
- Persistència amb `localStorage`

---

## Estructura del Projecte i Implementació DevOps

Durant aquesta pràctica s'ha completat el cicle complet de qualitat de programari, automatització i manteniment:

1. **Refactorització i Tests:**
   - Codi de JavaScript refactoritzat i modularitzat.
   - Integració del framework **Vitest** per a l'execució de tests unitaris i de components.
   - Comandament de tests: `npm test`

2. **Integració Contínua (CI):**
   - Workflow configurat a `.github/workflows/ci.yml`.
   - Execució automàtica de la instal·lació de dependències i tests en cada Pull Request mitjançant el job `Install Dependencies and Run Tests`.

3. **Protecció de la Branca `main`:**
   - Configuració de regles de protecció per exigir Pull Requests obligatòries.
   - Verificació d'estats obligatòria (`status checks` de la CI): 
     * **CI PASS** $\rightarrow$ Merge permès.
     * **CI FAIL** $\rightarrow$ Merge blocat automàticament.

4. **Desplegament Continu i GitHub Pages:**
   - Desplegament automàtic de l'aplicació web configurat mitjançant GitHub Actions (`.github/workflows/deploy.yml`).
   - Publicació automàtica a cada actualització de la branca `main`.

5. **Gestió de Dependències amb Dependabot:**
   - Configuració activa a `.github/dependabot.yml` per a la revisió periòdica (setmanal) d'actualitzacions de les dependències de l'ecosistema `npm` i de les accions de `github-actions`.

---

## Instal·lació i Execució Local

```bash
# Instal·lar les dependències
npm install

# Executar els tests unitaris
npm test

## Funcionalitats

- Crear tasques
- Completar tasques
- Eliminar tasques
- Filtrar tasques
- Veure estadístiques
- Persistència amb localStorage


## Instal·lació

```bash
npm install
```

## Tests

```bash
npm test
```

## Pràctica

Aquest projecte és el punt de partida per a una pràctica de DevOps amb GitHub.

Els alumnes hauran de refactoritzar el JavaScript, ampliar els tests i configurar GitHub Actions, Pull Requests, protecció de `main`, GitHub Pages i Dependabot.
