# Notre première application !

Tous nos outils étant installés, il est désormais temps de s'attaquer à notre première application. Ne prenez pas peur, rien de bien compliqué ici : nous allons juste cherche à afficher un traditionnel `Hello World !`, afin de saluer le nouveau monde qui s'ouvre à nous. Et vous verrez, ce n'est pas sorcier !

Dans un fichier portant l'extension `.pl`, insérez le code ci-dessous :
```perl6
# app.pl
use v6;

use Bailador;

get '/' => sub {
    "Hello World";
}

baile;
```
Comme vous avez pu le lire, mon fichier se nomme `app.pl`. Afin de lancer notre première application, dans un terminal, saisissez la commande suivante :
```
$ perl6 app.pl
Entering the development dance floor: http://127.0.0.1:3000
[2017-05-26T15:55:32Z] Started HTTP server.
```
Autrement dit, Bailador vous informe à sa manière qu'il est prêt !  
Pour le vérifier, rendez-vous avec votre navigateur à l'adresse indiquée, soit http://127.0.0.1:3000. Bailador vous souhaite donc la bienvenue ; et je me permets de faire de même : bienvenue à vous dans le monde de Bailador, en espérant que vous vous y plairez !

*A propos de l'extension .pl :  
Le fichier de mon application porte ici l'extension `.pl`, tout comme un fichier Perl standard. Vous pourrez trouver - et utiliser ! - d'autres alternatives, comme l'extension `.pl6`, qui peut notamment permettre de spécifier à certains éditeurs de texte l'utilisation de Perl 6. Au final, le résultat est le même !
*

*A propos du use v6...  
Vous aurez également remarqué que la première ligne de mon application est `use v6`. Cette première directive n'est pas obligatoire, mais permet de se prémunir d'erreurs incompréhensibles. En effet, si vous venez à lancer votre application avec Perl 5, vous obtiedrez uniquement un avertissement, précisant que vous ne pourrez pas lancer un code Perl 6 avec la version 5 de Perl. Forcément...
*

## Créer une application encore plus rapidement

### Grace au squelette de Bailador

...
