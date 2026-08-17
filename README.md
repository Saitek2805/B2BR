# B2broot
como esta recomendado, elijo debian en la útima versión disponible a 10 de agosto de 2026.

## Contraseñas:
#### Usuarios:


#### Encriptación de la partición del disco:



Requisitos Debian
https://www.debian.org/releases/stable/amd64/ch03s04.en.html

AppArmor Linux kernel
https://es.wikipedia.org/wiki/AppArmor

getent
https://man7.org/linux/man-pages/man1/getent.1.html

OpenSSH
https://en.wikipedia.org/wiki/OpenSSH

/etc/ssh/sshd_config y /etc/ssh/ssh_config
Archivo de configuración de SSH  sshd_config is the server. ssh_config is the client.

UFW
https://en.wikipedia.org/wiki/Uncomplicated_Firewall
denegar todas las ips menos 4242
https://serverfault.com/questions/648672/ufw-deny-all-incoming-except-ssh

Privilegios de sudo
https://documentation.suse.com/es-es/sles/16.0/html/SLES-sudo-configure-superuser-privileges/

porque sudoers.d
https://superuser.com/questions/869144/why-does-the-system-have-etc-sudoers-d-how-should-i-edit-it

TTY
https://unix.stackexchange.com/questions/4126/what-is-the-exact-difference-between-a-terminal-a-shell-a-tty-and-a-con

login.defs
/etc/login.defs
https://www.zonasystem.com/2020/04/gestion-de-las-politicas-de-contrasenas-en-linux-logindefs-pam-pwquality-cracklib.html

pam_pwquality
https://linux.die.net/man/8/pam_pwquality

/etc/pam.d/common-password

minlen=10 ➤ The minimum characters a password must contain.

ucredit=-1 ➤ The password must contain at least one capital letter. We must write it with a - sign, as this is how it knows that it refers to minimum characters; if we put a + sign it will refer to maximum characters.

dcredit=-1 ➤ The password must contain at least one digit.

lcredit=-1 ➤ The password must contain at least one lowercase letter.

maxrepeat=3 ➤ The password cannot have the same character repeated three consecutive times.

reject_username ➤ The password cannot contain the username within itself.

difok=7 ➤ The password must contain at least seven different characters from the last password used.

enforce_for_root ➤ We will implement this password policy for root.

passwd para cambiar la contraseña del usuario.
