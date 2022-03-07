# Первая настройка Git.

Оглавление

## Генерация SSH-ключа

1. Скачать и установить [`клиент Git`](https://git-scm.com/) на компьютер.

2. Запустить `Git-Bash`.

3. Выполнить команду генерации пары публичного и приватного ключей:
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

4. Ввести имя файла, которое будет использовано для ключа
```
Enter a file in which to save the key (/Users/you/.ssh/id_ed25519): <file-name>
```

5. Пароль можно не использовать, для этого нажать `Enter`:
```
> Enter passphrase (empty for no passphrase): [Press enter]
> Enter same passphrase again: [Press enter]
```


## Настройка публичного ключа:

1. Создать аакаунт на сайте [Git Hub](https://github.com)

2. Зайти в `Settings->SSH and GPG keys`.

3. Выбрать создать новый ключ `New SSH key`.

4. Написать заголовок ключа, поле `Title`.

5. В поле `Key` скопировать содержимое файла публичного ключа `<file-name>.pub`.

6. Сохранить ключ, нажав на кнопку `Add SSH key` и в всплывающем окне ввести пароль от сайта `Git Hub`.
