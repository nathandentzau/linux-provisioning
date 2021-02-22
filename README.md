# Nathan Dentzau's Pop!_OS 20.04 Provisioning

Hello 👋. This repository contains the Ansible playbook I use to provision my
computer that runs Pop!_OS 20.04. Hopefully this is a starting point for you to
configure your own computer with Ansible.

## Getting started

You'll want to find a way to copy this entire directory to the system you wish
to run this playbook on.

### Installing Ansible

Most like the system you want to run this playbook on does not have Ansible
installed. Run this script to get us going!

```bash
$ bin/setup
```

### Running the playbook for the first time

There's also a script to assist in running ansible. The first time you run the
playbook you'll need to supply the password of the user executing the script:

```bash
$ bin/run -K
```

The `-K` option will prompt Ansible to ask for the current user's password for
sudoer privileges.

### Running the playbook

After you've run the playbook once all you have to do is run:

```bash
$ bin/run
```

And you're provisioning!

## Notes

* This playbook is only meant to run on my machine and this I've hard coded some
  values in the playbook I would not normally hard code in a production
  playbook.
* Use at your own discretion please.
* I learned how to use Ansible from [@geerlinguy][]'s book back in 2016. I don't
  use it work anymore so I may be using outdated patterns.
* I stole the `git fixup` script from [@marcaddeo][].

[@geerlingguy]: https://github.com/geerlingguy
[@marcaddeo] https://github.com/marcaddeo
