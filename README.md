# Polaris packages feed

## Description

Ce feed correspond à la collection de paquetage utilisés dans Polaris Firmware.

## Usage

Ce feed n'est pas présent par défaut dans openwrt. Il est necessaire d'ajouter la ligne suivante dans feed.conf.default
Ensuite, pour installer tous les définitions des paquetages, executer:

./scripts/feeds update luci
./scripts/feeds install -a -p luci

Dans polaris-firmware ce feed est installé par défaut.
