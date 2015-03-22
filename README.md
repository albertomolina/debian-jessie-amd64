# debian-jessie-amd64
Minimal debian jessie vagrant box (amd64) for virtualbox provider build with veewee.

## Veewee

Veewee is a tool for easily (and repeatedly) building custom Vagrant base boxes, KVMs, and virtual machine images. Veewee it's available at [https://github.com/jedi4ever/veewee](https://github.com/jedi4ever/veewee)

Follow the [instructions](https://github.com/jedi4ever/veewee/blob/master/doc/installation.md) and install veewee

## Build your own debian jessie vagrant box

Clone this repository inside definitions directory and build your own vagrant box with:

    $ bundle exec veewee vbox build 'debian-jessie-amd64'
    $ bundle exec veewee vbox export 'debian-jessie-amd64'

Customizations can be made proviously modifying properly preseed.cfg file

**Note**: This box doesn't include neither chef nor puppet agents.

## Use this box

Do you want just to use a debian jessie vagrant box? This box is available for download at [https://vagrantcloud.com/albertomolina/boxes/debian-jessie-amd64](https://vagrantcloud.com/albertomolina/boxes/debian-jessie-amd64). You can add it locally with:

    vagrant box add --name albertomolina/debian-jessie-amd64 https://vagrantcloud.com/albertomolina/boxes/debian-jessie-amd64
