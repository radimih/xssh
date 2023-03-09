# `xssh`

Bash-скрипт для организации SSH-соединений.

Скрипт зависит от следующих приложений:

- `ranger`
- `sshpass`
- [`yq`](https://github.com/kislyuk/yq)

## Профили соединений

Файлы профилей соединений должны располагаться в каталоге `~/.ssh/connections`
и в его подкаталогах.

Один YAML-файл описывает одно SSH-соединение. Формат:

```yaml
name: <произвольное название>
host: <IP или DNS-имя хоста>
user: <имя пользователя, под которым будет создано SSH-соединение>
[password: <пароль>]
```
