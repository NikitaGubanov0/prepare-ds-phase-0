# GitHub
Для начала посмотри [лекцию по github](https://youtu.be/4TRClQ7rttw)

GitHub - это [cистема управления версиями](https://ru.wikipedia.org/wiki/Система_управления_версиями) с социальной составляющей. В соцсети вы выкладываете фотографии, а тут исходный код. Это ещё и самая большая площадка для opensource проектов. Веб-сервис основан на [системе](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) контроля версий [Git](https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F). Ну и конечно, вы можете сделать свою гитхаб страницу своим [*резюме*](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme).

## Настройка доступа по [SSH](https://ru.wikipedia.org/wiki/SSH)
Для начала настроим доступ к репозиториям аккаунта. 

### Пример для linux
Про команды, для работы в терминале и про сам bash, можно подробнее посмотреть [здесь](bash.md).

- откройте терминал (`Ctrl + Alt + T`) на своём компьютере и выполните ряд команд
   * `обновление списков пакетов для обновлений`
   * `установка пакета ssh`
    ``` 
    sudo apt update    
    sudo apt-get install ssh    
    ```
 
**`на macos начинайте отсюда`**
- далее мы запустим команды, для генерации собственных SSH-ключей (ed25519 - это [крипто-схема](https://ru.wikipedia.org/wiki/EdDSA))
    ```
    ssh-keygen -t ed25519 -C "подставь сюда свою почту, на которую регистрировался github и кавычки оставь"
    ```
   - нажми на Enter три раза (так проще, заполнять ответы/фразы не обязательно)



Теперь в корневой папке твоего компьютера есть [*скрытая*](https://nextontext.ru/linux-i-os-x/646-skrytye-fajly-i-papki-v-ubuntu) папка `.ssh` (на mac `command+shift+.`), внутри лежат два файла `id_ed25519` и `id_ed25519.pub`. Первый - твой приватный ключ устройства, второй - публичный, его мы и будем использовать в качестве ключа на странице добавления публичных ключей в аккаунт [GitHub](https://github.com/settings/keys).

- можно запустить [команду чтения](https://losst.ru/komanda-cat-linux) содержимого файла `cat .ssh/id_ed25519.pub`, 
- выделить и скопировать из терминала, через сочетание клавиш `ctrl+shift+c`, содержимое публичного ключа (на mac просто `command+c`)
- копируем всю строку от включительно `ssh-ed25519 ...` и до `... ваша@почта.com` включительно 
- пора скопировать ключ на [GitHub](https://github.com/settings/ssh/new)
- название `Title` можно задать любое, обычно такое, чтобы вам было понятно, о ключе с какого компьютера идёт речь

...


## Создаём связанную копию репозитория - Fork 

Когда ваша система уже настроена, получен и подключен SSH-ключ, вам ничего не мешает создать копию этого репозитория у себя в аккаунте. Нужно лишь нажать на кнопку `Fork` сверху слева на главной странице репозитория - `https://github.com/Elbrus-DataScience/ds-phase-0`

Теперь можно перейти на свою страницу c репозиториями `https://github.com/USER?tab=repositories`, *здесь и далее* `USER` – ваш ник в GitHub. Второй вариант - вы кликаете на фото профиля в правом верхнем углу и переходим во вкладку `Your profile` или `Your repositories` для доступа к странице аккаунта и репозиториев соответственно.

- переходим на страницу вашего форка (в поле ввода браузера должно быть `https://github.com/USER/ds-phase-0`)
<!-- заменить на ds_online -->
- здесь нажимаем на *зелёную* кнопку <span style="color: green;">**Code**</span>
- выбираем вкладку <span style="text-decoration:underline">**SSH**</span>
- *копируем* ссылку на репозиторий (она должна быть такого вида: `git@github.com:USER/ds-phase-0.git`)
<!-- заменить на ds_online -->

Идём выполнять команды git в терминале своего [компьютера](git.md)

#### Ссылки
- 📑  Инструкция по генерации [ключа SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
- 📝 Пример соединения серверов по SSH от [DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-use-ssh-to-connect-to-a-remote-server-ru)
- 📝 Установка и настройка SSH от [REG](https://help.reg.ru/hc/ru/articles/4408047830033-Как-установить-и-настроить-SSH)
- 📑 Статья про fork на [GitHub](https://docs.github.com/en/get-started/quickstart/fork-a-repo)




