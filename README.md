MacOS Defaults module
=====================

This is a fork of Ansible's osx_defaults module.
It allows users to read, write, and delete MacOS preferences from Ansible.
This fork is based on Etienne Desautels' fork, using Foundation/CoreFoundation.
It adds support for nested keys and values, and support for all types.


Usage
-----

Until this gets adopted as an official Ansible module (or Ansible accepts these
changes to the osx_defaults module), just copy the `macos_defaults.py` file
somewhere that Ansible will find it. The easiest way to do that is to put it
in the `library` directory as a sibling to your Ansible playbook. You might
even just clone this repository as a submodule named `library`, if you only
need this one module. You can do that with:

~~~ shell
git submodule add git@github.com:boochtek/macos_defaults.git library
~~~
