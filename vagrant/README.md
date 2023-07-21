# vagrant

This folder contains two Vagrantboxes for spinning up a complete environment.

## Requirements

- at least 21 GB of free memory
- [HashiCorp Vagrant](https://vagrantup.com)
- [Oracle VirtualBox](https://virtualbox.org) or XEN/KVM (*and the `vagrant-libvirt` plugin*)

## Usage

Spin-up the environment:

```command
$ vagrant up
```

This can take **up to 60 minutes**, depending on your machine and internet connection.

Afterwards, you can use the web-interface using one of the following URLs:

- [https://localhost:8443 (VirtualBox)](https://localhost:8443)
- [https://192.168.23.100 (XEN/KVM)](https://192.168.23.100)

Username and password: `admin` / `chad`

Shutdown the VMs:

```command
$ vagrant halt
```

Destroy the VMs once you're finished:

```command
$ vagrant destroy
```
