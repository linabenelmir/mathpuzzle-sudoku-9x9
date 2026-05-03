Projet Sudoku 9x9 - version corrigee

Corrections faites:
1. pom.xml corrige pour Spring Boot 3.4.5.
2. Dependency web corrigee: spring-boot-starter-web.
3. H2 garde en runtime, avec console active via application.properties.
4. Port fixe: 8090.
5. Suppression du dossier/config H2ConsoleConfig inutile.

Instructions dans Eclipse:
1. File > Import > Existing Maven Projects.
2. Choisir le dossier mathpuzzle.
3. Right click sur le projet > Maven > Update Project.
4. Cocher Force Update of Snapshots/Releases puis OK.
5. Project > Clean.
6. Run As > Maven build...
7. Dans Goals, ecrire:
   spring-boot:run -Dspring-boot.run.jvmArguments="-Xmx512m -XX:MaxMetaspaceSize=256m"

Application:
http://localhost:8090

H2 Console:
http://localhost:8090/h2-console

Connexion H2:
JDBC URL: jdbc:h2:file:./data/mathpuzzle-db
User Name: sa
Password: laisser vide

Pour la video:
- Montrer login/register.
- Montrer home, score et niveau.
- Lancer une partie Sudoku.
- Sauvegarder/Reprendre.
- Montrer h2-console ou application.properties si la console H2 ne s'ouvre pas sur votre machine.
