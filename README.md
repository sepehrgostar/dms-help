# dms-help
manage email server help


# commands CLI
    COMMAND email :=
        setup email add <EMAIL ADDRESS> [<PASSWORD>]
        setup email update <EMAIL ADDRESS> [<PASSWORD>]
        setup email del [ OPTIONS... ] <EMAIL ADDRESS> [ <EMAIL ADDRESS>... ]
        setup email restrict <add|del|list> <send|receive> [<EMAIL ADDRESS>]
        setup email list

    COMMAND alias :=
        setup alias add <EMAIL ADDRESS> <RECIPIENT>
        setup alias del <EMAIL ADDRESS> <RECIPIENT>
        setup alias list

    COMMAND quota :=
        setup quota set <EMAIL ADDRESS> [<QUOTA>]
        setup quota del <EMAIL ADDRESS>

    COMMAND dovecot-master :=
        setup dovecot-master add <USERNAME> [<PASSWORD>]
        setup dovecot-master update <USERNAME> [<PASSWORD>]
        setup dovecot-master del [ OPTIONS... ] <USERNAME> [ <USERNAME>... ]
        setup dovecot-master list

    COMMAND config :=
        setup config dkim [ ARGUMENTS... ]

    COMMAND relay :=
        setup relay add-auth <DOMAIN> <USERNAME> [<PASSWORD>]
        setup relay add-domain <DOMAIN> <HOST> [<PORT>]
        setup relay exclude-domain <DOMAIN>

    COMMAND fail2ban :=
        setup fail2ban 
        setup fail2ban ban <IP>
        setup fail2ban unban <IP>
        setup fail2ban log

    COMMAND debug :=
        setup debug fetchmail
        setup debug login <COMMANDS>
        setup debug show-mail-logs


# upgrade emailsever from docker
 
```
sudo apt update
sudo apt upgrade

docker compose pull
docker compose down
docker compose up -d
```
