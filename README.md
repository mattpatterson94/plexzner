## Plexzner

Ansible setup for setting up Plex and torrent client

### Requirements

* Ansible

### Includes

* Plex
* Plex auto updater
* Tautulli (Plex stats)
* Transmission client

### Installation

1. Copy example files

```
cp .envrc.example .envrc
cp inventory.example inventory
```

2. Modify envrc and inventory to have the values required

3. Run Ansible via:

```
ansible-playbook -i inventory initial-server-setup.yml
```

### Considerations

* This guide assumes UFW is installed. I'm not a pro at ansible so I kind of jigged it in.
* Transmission requires a user to already hae been created. I use the ruler user that is set for the base role. It has to be set in multiple places (coupling bleh)
