# Pwnabox - pwning with whales!

Some tools integrated image for easy CTF or education. It also could be used for sandboxing.

## Included tools

* Pwntools (https://github.com/Gallopsled/pwntools)
* pwntools-ruby (https://github.com/peter50216/pwntools-ruby)
* Radare2 (https://github.com/radare/radare2)
  * r2pm
  * r2dec (https://github.com/wargio/r2dec-js)
* one_gadget (https://github.com/david942j/one_gadget)
* GDB addons
  * pwndbg (https://github.com/pwndbg/pwndbg)
  * GEF (https://github.com/hugsy/gef)
  * Peda (https://github.com/longld/peda)
    * Peda-heap (https://github.com/Mipu94/peda-heap)
* tracers
  * strace
  * ltrace
* packer
  * upx

## Getting Started

### Dependencies:

- Docker
- Docker Compose

### Clone this project

```bash
> git clone https://github.com/RoiKlevansky/pwnabox.git
> cd pwnabox
```

### Installation

After the command starts it will print the name of the created container,
keep note of the name as you will need to use it when getting in.

```bash
> docker-compose up -d
```

### Running

```bash
> docker exec -it <Containter Name> zsh
```

Default crednitals are: ```pwner:pwner```.

## Special Commands

This image uses a script named [gdb-peda-pwndbg-gef](https://github.com/RoiKlevansky/gdb-peda-pwndbg-gef) which lets you easly run peda, pwndbg and gef
on the same machine. Use one of the commands below to launch the corresponding GDB environment:

```bash
> gdb-peda
> gdb-peda-intel
> gdb-peda-arm
> gdb-pwndbg
> gdb-gef
```
