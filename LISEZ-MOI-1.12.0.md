# Correctif français pour Karakeep mobile 1.12.0

`karakeep-fr-1.12.0.patch` s'applique à la branche principale de Karakeep au commit `93b478314dcf753fcf549f3482e34447db7319d4` (appli mobile 1.12.0). Il traduit environ 540 textes de l'interface et nomme l'appli « Karakeep FR » (identifiant `app.hoarder.hoardermobile.fr`) pour qu'elle cohabite avec celle du Play Store.

Le correctif existant `karakeep-fr.patch` (v0.33.2, appli 1.10.0) n'est pas modifié.

## Compiler avec le workflow « Compiler Karakeep FR »
Le workflow applique `karakeep-fr.patch` en dur. Pour ce nouveau correctif, il faut deux changements dans `.github/workflows/build.yml` :
1. à l'étape « Appliquer la traduction française », remplacer `../fr/karakeep-fr.patch` par `../fr/karakeep-fr-1.12.0.patch` ;
2. lancer le workflow avec la version `93b478314dcf753fcf549f3482e34447db7319d4` (le champ accepte n'importe quelle référence Git).

Ces changements ne sont pas faits ici pour ne pas casser le workflow actuel.
