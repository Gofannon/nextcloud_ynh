### Comment utiliser la commande CLI

`sudo -u __APP__ php__YNH_PHP_VERSION__ --define apc.enable_cli=1 __INSTALL_DIR__/occ ...`

ou utilisez `sudo yunohost app shell __APP__` puis `php occ ...`

### Configurer l'intégration d'ONLYOFFICE

#### Avec l'application YunoHost (support ARM64, meilleures performances)

Pour  de meilleures performances et le support de ARM64 (Raspberry Pi, OLinuXino...), installez l'app YunoHost ONLYOFFICE, voir le tutoriel dans la [doc du paquet onlyoffice_ynh](https://github.com/YunoHost-Apps/onlyoffice_ynh/blob/master/README_fr.md#configuration-de-onlyoffice-server)

#### Alternative: Avec l'application Nextcloud (pas de support ARM, performances limitées)

Nextcloud inclut une intégration directe de ONLYOFFICE (un éditeur de texte enrichi en ligne) via une application Nextcloud.
Pour l'installer et la configurer :
- Installez l'application *Community Document Server* dans votre Nextcloud. C'est la partie qui fait tourner un serveur ONLYOFFICE.
- Installez l'application *ONLYOFFICE*. C'est la partie cliente qui va se connecter au serveur ONLYOFFICE.
- Ensuite dans les Paramètres -> ONLYOFFICE (`https://__DOMAIN____PATH__/settings/admin/onlyoffice`), si vous voulez configurer quels formats de fichier s'ouvrent avec ONLYOFFICE.

*NB : l'app Nextcloud ONLYOFFICE Community Document Server n'est disponible que sous architecture x86
