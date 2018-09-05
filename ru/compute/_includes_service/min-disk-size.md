>[!NOTE]
>
>Значение `min-disk-size` должно быть больше объема исходных данных в образе и больше размера виртуального диска, указанного в образе.
>
>Если указать значение `min-disk-size` меньше допустимого, то произойдет ошибка и образ не будет создан. В описании ошибки будет указано минимальное значение в байтах, например `Minimal disk size should be greater or equal than 10737418240`.
>
>Если не указать `min-disk-size`, будет использовано минимальное значение.