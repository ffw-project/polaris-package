# Polaris packages feed

## Description

Ce feed correspond à la collection de paquetage utilisés dans Polaris Firmware.

## Usage

Ce feed ainsi que toute les définitions de chaque paquet sont installés par défaut dans Polaris Firmware. En revanche il n'est pas présent dans openwrt et il est nécessaire d'ajouter la ligne suivante dans feed.conf.default.

src-git polaris https://github.com/ffw-project/polaris-package.git

Ensuite, pour installer toutes les définitions des paquetages dans openwrt, exécuter:

./scripts/feeds update polaris
./scripts/feeds install -a -p polaris
