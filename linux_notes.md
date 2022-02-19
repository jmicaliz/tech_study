# Linux Notes

## Setup Static IP for Ubuntu
#ip #ubuntu #static #network

More information on configuring networking here: https://www.swiftstack.com/docs/install/configure_networking.html

Although, I haven’t tried it yet.

## Check network configuration
#ip #network #command

[ip](https://linux.die.net/man/8/ip)

## Check stuff about service
#service #status #ubuntu

```bash
service <service_name> <status|start|stop>
```

https://askubuntu.com/questions/903354/difference-between-systemctl-and-service-commands

Sometimes use systemctl like:

```bash
systemctl <command> <service_name>
```

`service` is a wrapper for `systemctl`

## Ubuntu service at startup
#service #startup #ubuntu

https://askubuntu.com/questions/9382/how-can-i-configure-a-service-to-run-at-startup

```bash
man update-rc.d
```

## Update Ubuntu
#ubuntu #update #upgrade

```bash
sudo apt-get upgrade
```

## Check list of services that start/don’t at start up Ubuntu
#startup #services #ubuntu

```bash
systemctl list-unit-files --type=service
```

## Create Symbolic Link
#symbolic #link #command

[Notes on symbolic link](https://baptiste-wicht.com/posts/2012/09/linux-symbolic-links-hard-links.html)

```bash
ln -s <source_file/dir> <link_name>
```

## Mount drobo
#mount

https://community.spiceworks.com/topic/1896820-mounting-a-drobo-share-in-linux

Then after run:
```bash
sudo mount -a
```

## Find out stuff about commands
#search #find

[apropos](http://www.linfo.org/apropos.html)

## Reboot Ubuntu from Command Line
#reboot #cli #ubuntu #restart

```bash
sudo reboot
```

or

```bash
sudo shutdown -r now
```

## View All Users
#users #ubuntu

```bash
cut -d: -f1 /etc/passwd
```
[More information](https://askubuntu.com/questions/410244/a-command-to-list-all-users-and-how-to-add-delete-modify-users)
