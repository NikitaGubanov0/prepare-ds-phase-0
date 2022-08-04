# Bash Envs

* Откройте терминал в директории ds-phase-0/learning/done/
* Создайте файл `02-bash-envs.sh`* 
* Создайте `02-environment.yml`**
* Загрузите ответы на github в свой репозиторий

*это исполняемый файл скрипта [bash](../01-general/bash.md)

**[YAML](https://ru.wikipedia.org/wiki/YAML)

### Задание 01:
В файле `02-bash-envs.sh` напишите команды для создания окружения через `pip venv`.
Окружение должно содержать библиотеки `pandas`, `scikit-learn`, `matplotlib`, `seaborn`.
Имя окружения должно быть `EDA` (кстати, как это расшифровывается?)

### Задание 02:
В файле `02-environment.yml` напишите команды для создания окружения через [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
Окружение должно содержать библиотеки `aiogram`, `flask`.
Имя окружения должно быть `production`.

## Итог
+ 2 файла для создания окружений в формате sh-скрипта и yaml-файла. Эти файлы вы будете использовать и редактировать в процессе обучения для создания своих проектов в будущем.

### Задание 03 со звёздочкой:
Создайте sh-скрипт, который собирает данные о том, какие установлены библиотеки в Python окружении и создаёт файл environment.yml с этими данными, для установки именно этих библиотек в окружении conda.