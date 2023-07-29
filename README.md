# dms-help
document manage email server 
### login to ubuntu server with putty on ssh
in windows use `putty` and in ubuntu use `terminal console`

https://www.putty.org/

## sample docker command

after login use command CLI like bellow
`sudo docker exec mailserver setup email add info@site.com PASSWORED`

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

    COMMAND fail2ban :=
        setup fail2ban 
        setup fail2ban ban <IP>
        setup fail2ban unban <IP>
        setup fail2ban log

if you have same problems in usage this help plese contact to support or send email to us va6893@gmail.com
