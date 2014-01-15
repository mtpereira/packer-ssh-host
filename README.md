packer-ssh-host
===============

Packer template for a SSH host.

For now the only builder configured is Digital Ocean, which will output a snapshot.

Usage
=====

Use one (or more) files to define your variables and include them with _-var-file_ option of packer.

At the moment, there are the following variables:

* do_api_key (_required_): API key for Digital Ocean.
* do_client_id (_required_): Your Digital Ocean client ID.
* do_region_id (optional): Digital Ocean droplet zone (defaults to Amsterdam 2, "5").
* do_size_id (optional): Digital Ocean droplet size (defaults to 512 MB, id "66").
* hostname (_required_): Hostname, which will also be droplet's name in Digital Ocean.
* user (_required_): SSH user.
* password (_required_): SSH user's password.
