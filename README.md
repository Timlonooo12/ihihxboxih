<p align="center">
  <img src="logo.png" width="160" alt="Ambxs">
</p>

<h1 align="center">Ambxs Achievement Unlocker</h1>

<p align="center">
  <a href="https://github.com/Timlonooo12/ihihxboxih/raw/main/AmbxsAchievementUnlocker.exe"><b>⬇ Télécharger AmbxsAchievementUnlocker.exe</b></a>
</p>

## Installation

Il n'y a rien à installer :

1. Téléchargez **AmbxsAchievementUnlocker.exe** avec le lien ci-dessus.
2. Lancez le fichier.

Le runtime .NET est inclus dans l'exe.

- **Avertissement Windows SmartScreen :** l'exe n'est pas signé. Cliquez sur « Informations complémentaires » puis « Exécuter quand même ».
- **Configuration requise :** Windows 10 ou 11 (64 bits), avec WebView2 pour la fenêtre de connexion Microsoft. WebView2 est déjà présent sur les Windows à jour.

## Utilisation

1. Ouvrez la page **Batch Unlock**.
2. Cliquez sur **Add account** et connectez-vous avec un compte Microsoft / Xbox. Recommencez pour chaque compte que vous voulez utiliser en même temps.
3. Choisissez un mode :
   - **Plan by desired Gamerscore** : continue jusqu'à ce que le Gamerscore demandé soit débloqué et vérifié, par exemple `1000000`.
   - **Plan by title count** : traite un nombre de jeux donné.
4. Cliquez sur **Start selected**.

Chaque compte affiche son Gamerscore vérifié, le montant restant et le temps estimé.

La connexion classique via la fenêtre Microsoft ou `/connect` utilise le stockage chiffré du programme et permet le renouvellement tant que la session reste valide. Une session expirée doit être reconnectée ; les progrès du lot sont conservés.

## Connexion multicomptes depuis Discord

Dans **Settings → Discord**, renseignez le **Bot Token** et vos identifiants dans **Owners (Discord user IDs)**, cliquez sur **Apply**, puis activez **Enable Discord Bot**. La commande `/connect_accounts` est réservée aux owners et aux co-owners ajoutés avec `/addowner`.

Collez un compte par ligne au format `mail:pass:mail2fa:pass2fa`, ou joignez un fichier `.txt` dans l’option `file`. La vérification e-mail utilise l’API REST de mail.tm, pas IMAP. La boîte de vérification doit déjà être associée au compte Microsoft et vous appartenir. Après connexion, vérifiez les comptes avec `/accounts`, puis utilisez votre `/unlock` habituel pour les sélectionner. Cette nouvelle connexion ne lance aucun déblocage et ne modifie pas `/unlock`.

**Les identifiants du formulaire transitent par Discord et le bot.** Utilisez uniquement vos comptes ou des comptes explicitement autorisés. Préférez `/connect` pour ne pas communiquer de mots de passe au bot. Les nouvelles sessions par identifiants restent en mémoire et doivent être reconnectées après un redémarrage ou leur expiration. Pour CAPTCHA, SMS et Authenticator, utilisez `/connect` et validez sur Microsoft : la connexion par liste ne traite pas ces challenges. Le parcours par identifiants peut aussi échouer si les pages Microsoft changent.

Le build a été compilé et les tests simulés ont réussi. Ces tests ne constituent pas une validation de connexion réelle à un compte Microsoft.

## Vérification

Empreinte SHA-256 de l'exe actuel :

```
6dc7748249a124dc4d9f04d64fb9c127cb137b1e757f994d601a0804ad3a8f33
```

## Licence

Basé sur [Xbox Achievement Unlocker](https://github.com/Fumo-Unlockers/Xbox-Achievement-Unlocker), distribué sous licence **GPL-3.0** (voir [LICENSE](LICENSE)). Le code source de cette version est disponible sur demande, conformément à la licence.
