# Polaris packages feed

## Description

Ce feed correspond à la collection de paquets utilisés dans Polaris Firmware.

## Usage

Les paquets de ce feed sont installés par défaut dans Polaris Firmware. 

En revanche, pour une utilisation dans Openwrt il est nécessaire d'ajouter dans feed.conf.default la ligne suivante.

src-git polaris https://github.com/ffw-project/polaris-package.git

Ensuite, pour installer toutes les définitions des paquetages dans openwrt, exécuter:

./scripts/feeds update polaris
./scripts/feeds install -a -p polaris

Les paquets sont désormais présents dans le menuconfig.
