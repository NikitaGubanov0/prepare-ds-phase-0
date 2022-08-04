# Если что-то пошло не так 
*и хочется написать ментору в личные сообщения*
____

## Проверь описание ошибки
Прочти описание ошибки. Ту часть, которая указывает на невозможность чего-то, например:

        
            1 import numpy as np
        ----> 2 pd.DataFrame()
            3 ...

            NameError: name 'pd' is not defined
        
- `---->` стрелка, которая указывает на строку в коде, вызывающую ошибку
- описание ошибки означает, что переменной pd не существуют, то есть выше в коде нет инструкции, которая задаёт эту переменную

Как действовать в подобных случаях: 
    
- необходимо понять из ошибки, что не так с кодом
- исправить недостающие инструкции

## Если проблема неочевидна
Попробуй поискать решение в документации библиотеки или модуля: 
- посмотри подсказки – **docstring** функции, в которой ошибка
- или иди на **официальный** сайт документации, найди тот класс/метод/функцию/ которая используется в коде, где возникает ошибка
- посмотри, **какие аргументы необходимы**, какого они должны быть типа данных и прочие параметры, в которых возможно допустить ошибку
- проверь свой код на соответствие: что **ты подаёшь на вход** и того, что **необходимо** подавать
- посмотри примеры кода, если такие представлены в документации и сверь со своим

## Всё верно написано, но ошибка на месте – проверь код на опечтки и последовательность
Если по описанию не получается исправить ошибку, то попробуй просто пройтись с **самого начала** файла/ноутбука по каждой строке и проверить:

- все ли необходимые библиотеки/модули были **импортированны**
- все ли ячейки в ноутбуке **расположены в нужном порядке** и при этом **запущены** (!)
- перепроверь **имена переменных**, которые ты передаёшь в метод/функцию

## Если всё это не помогает
Загугли описание ошибки, NameError или код ошибки.
Делай это обязательно в google.com, на английском языке. 

## Возможно поможет утка
[Rubber duck debugging 🐥](https://ru.wikipedia.org/wiki/Метод_утёнка)

## Спроси коллег по обучению
Возможно они уже сталкивались с этой ошибкой.

- Если кто-то уже сумел исправить - замечательно! Вы оба/обе прекрасны!
- Если коллегу тоже беспокоит эта неисправленная ошибка - перепроверьте код друг друга
- И если всё это не помогло - обязательно пишите и просите помощь у ментора! Тегайте его через "собачку" @.

## Как задать вопрос ментору?
Вопросы наиболее **продуктивно и эффективно** формулировать следующим образом:
 - подробное **описание задачи** (что нужно получить, что было сделано, где проблема)
 - **примеры кода** до и после ошибки/проблемы, в виде скриншотов, например или `в блоке code`
 - **что и как пробовал найти**, чтобы решить проблему (обязательный пункт!)
 - что посоветовали **коллеги** по обучению (совместная работа крайне важна)

___
        Весь алгоритм на одну ошибку должен занимать не более получаса
