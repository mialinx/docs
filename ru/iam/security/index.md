# Безопасность и управление доступом

Пользователь Яндекс.Облака может выполнять только те операции над ресурсами, которые разрешены назначенными ему ролями. Пока у пользователя нет никаких ролей, все операции ему запрещены.

Чтобы разрешить доступ к ресурсам сервиса [!KEYREF iam-full-name] (сервисным аккаунтам и ключам доступа к ним), назначьте пользователю нужные роли из приведенного ниже списка. Вы можете назначить пользователю роль на сам сервисный аккаунт, на каталог, в котором находится аккаунт, или на все облако — права доступа в Яндекс.Облаке наследуются.


> [!NOTE]
>
> Подробнее о наследовании ролей читайте в разделе [[!TITLE]](../../resource-manager/concepts/resources-hierarchy.md#access-rights-inheritance) документации сервиса [!KEYREF resmgr-full-name].


## Назначение ролей

Чтобы назначить пользователю роль на облако или каталог:

[!INCLUDE [grant-role-console](../../_includes/grant-role-console.md)]

## Роли

Ниже перечислены все роли, которые учитываются при проверке прав доступа в сервисе [!KEYREF iam-short-name].

### Сервисные роли

_Сервисные роли_ — роли, дающие доступ к ресурсам определенного сервиса. При проверке прав доступа к ресурсам [!KEYREF iam-short-name] учитываются сервисные роли [!KEYREF resmgr-name].

[!INCLUDE [cloud-roles](../../_includes/cloud-roles.md)]

### Примитивные роли

Примитивные роли можно назначать на любой ресурс в любом сервисе.

#### [!KEYREF roles-viewer]

Пользователь с ролью `[!KEYREF roles-viewer]` может просматривать информацию о ресурсах, например получить список ключей доступа для сервисного аккаунта.

#### [!KEYREF roles-editor]

Пользователь с ролью `[!KEYREF roles-editor]` может управлять любыми ресурсами, например создать сервисный аккаунт или ключи доступа для него.

Помимо этого роль `[!KEYREF roles-editor]` включает в себя все разрешения роли `[!KEYREF roles-viewer]`.

#### [!KEYREF roles-admin]

Пользователь с ролью `[!KEYREF roles-admin]` может управлять правами доступа к ресурсам, например разрешить другим пользователям использовать сервисные аккаунты или просматривать информацию о них.

Помимо этого роль `[!KEYREF roles-admin]` включает в себя все разрешения роли `[!KEYREF roles-editor]`.
