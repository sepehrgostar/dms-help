# dms-help
document manage email server 
### login to ubuntu server with putty on ssh
in windows use `putty` and in ubuntu use `terminal console`

https://www.putty.org/

## sample docker command

after login use command CLI like bellow
`docker exec mailserver setup email add info@site.com PASSWORED`

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

if you have same problems in usage this help plese contact to support or send email to us va6893@gmail.com
