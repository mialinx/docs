# Работа с виртуальной машиной на базе публичного образа

## Подключение по SSH {#connect}

[!INCLUDE [vm-connect-ssh](../../../_includes/vm-connect-ssh.md)]

## Подключение по логину и паролю {#logins-passwords}

Вы можете подключиться к виртуальной машине по логину и паролю, когда она будет запущена.

[!INCLUDE [vm-connect-ssh-linux-note](../../../_includes/vm-connect-ssh-linux-note.md)]

Получить логины и пароли для виртуальных машин на базе публичного образа можно с помощью команды:

```
$ sudo cat /root/default_passwords.txt
```

Если аутентификация по паролю не предусмотрена, файла с паролями не будет.

## Использование протокола SSL {#ssl}

Чтобы использовать SSL, самостоятельно сгенерируйте SSL-сертификат и настройте веб-сервер для работы с ним.

## Фильтрация сетевого трафика {#network-filter}

На виртуальных машинах на базе публичного образа открыты только порты, необходимые для настройки и работы предустановленного программного обеспечения.

Вы можете посмотреть список открытых портов для конкретной виртуальной машины при [подключении по SSH](../vm-control/vm-connect-ssh.md). Чтобы открыть дополнительные порты, воспользуйтесь утилитой `iptables`.

## Установка обновлений {#updates}

На виртуальных машинах на базе публичного образа операционная система и программное обеспечение не обновляются автоматически. Вы можете обновлять их самостоятельно.
