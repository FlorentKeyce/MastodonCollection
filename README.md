# Ansible Mastodon Collection

Note mise à jour 2024 : ce playbook n'est pas totalement fonctionnel, il manque un partage de fichiers entre le serveur Mastodon et le frontal web (nginx).

## Usage

```
ansible-playbook playbook-mastodon.yml
```
Nécessite un accès root aux machines avec accès SSH sans mot de passe.

Une fois le premier utilisateur crée en interface web, lui donner les droits de propriétaire :
```
RAILS_ENV=production /home/mastodon/live/bin/tootctl accounts modify florent --role Owner
```
(https://docs.joinmastodon.org/admin/tootctl/)

## Notes

Mastodon est codé en Ruby et JavaScript (framework NodeJS).

Yarn : Package Manager NodeJS

Corepack : Experimental tool to help with managing versions of your NodeJS package managers (installé avec NodeJS)

Rbenv : Version manager tool for Ruby

Gem : (RubyGems) Package Manager Ruby (installé avec Rbenv)

Bundler (bundle command) : provides a consistent environment for Ruby projects by tracking and installing the exact gems and versions that are needed (installé avec Gem)


## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
