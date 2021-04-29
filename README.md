# misp-box

| License | Versioning | Build |
| ------- | ---------- | ----- |
| [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) | [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release) | [![Build status](https://ci.appveyor.com/api/projects/status/vjocnhar8uvvykbe/branch/master?svg=true)](https://ci.appveyor.com/project/nikAizuddin/misp-box/branch/master) |

Developer box for [MISP](https://github.com/MISP/MISP).


## Creating Vagrant Box

Copy example pillar file for MISP. Optionally you may want to edit the values in the `misp.sls`:
```
$ cp -v salt/roots/pillar/misp.sls.example salt/roots/pillar/misp.sls
```

Copy vagrant file from `vagrant/examples/` and then create the vagrant box (you can change to `--provider=virtualbox` if you want to use Oracle VirtualBox provider):
```
$ cp -v vagrant/examples/Vagrantfile.misp-box.fedora-33.x86_64.example vagrant/Vagrantfile.misp-box
$ vagrant up --provider=libvirt
```

Provision the vagrant box:
```
$ vagrant ssh misp-box -- sudo salt-call state.highstate
```

Build and deploy MISP:
```
$ vagrant ssh misp-box -- sudo salt-call state.sls misp
```


## Initializing MISP

First-time login:
* email: `admin@admin.test`
* password: `admin`

To initialize feeds:
1. Go to `Sync Actions` > `List Feeds`.
1. Click `Load default feed metadata`.
1. Select and enable all feeds.
1. Click `Fetch and store all feed data`. No need to cache.

To initialize galaxies:
1. Go to `Galaxies` > `List Galaxies`.
1. Click `Update Galaxies`.
