Nécessite un accès root aux machines avec accès SSH sans mot de passe.

#Configuration sudo sans mot de passe dans /etc/sudoers.d/openit-nopasswd :
#openit ALL=NOPASSWD: ALL

Une fois le premier utilisateur crée en interface web, lui donner les droits de propriétaire :
RAILS_ENV=production /home/mastodon/live/bin/tootctl accounts modify florent --role Owner
(https://docs.joinmastodon.org/admin/tootctl/)

Mastodon est codé en Ruby et JavaScript (framework NodeJS).

Glossaire : 

Yarn : Package Manager NodeJS
Corepack : Experimental tool to help with managing versions of your NodeJS package managers
Rbenv : Version manager tool for Ruby
Gem : (RubyGems) Package Manager Ruby
Bundler (bundle command) : provides a consistent environment for Ruby projects by tracking and installing the exact gems and versions that are needed
