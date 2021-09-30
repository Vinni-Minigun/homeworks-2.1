# Git. README.md (пример)

# Название проекта

Короткое описание проекта

## *Начало работы*

Небольшой набор инструкций, объясняющий, как получить копию этого проекта для запуска на локальном ПК.

### Prerequisites

Что нужно установить на ПК для использования (например: Git, браузер и т.д.).

```
Примеры
```

### Установка и запуск

Пошаговый процесс установки и запуска

```
Примеры
```

## *Лицензия*

Опишите условия лицензии

```
css
# Домашнее задание к лекции «История и работа с ветками»

## Задача №1 - Создание веток

### Легенда

Маркетологи поставили задачу — необходимо дописать текст на главной странице проекта, в котором рассказывается с какими компаниями мы уже работаем. Но текст пока находится на согласовании. Его нужно будет добавить в новую ветку, чтобы пользователи его пока не видели, но маркетологи понимали, хорошо ли он выглядит. Скопируйте текст из **Приложения №1** и вставьте его в файл `README.md`.

Для разработки новых функций необходимо использовать ветки (branches) чтобы случайно в ходе разработки не сломать существующий функционал. Ваша задача — создать новую ветку и в ней произвести все изменения.

<details>
<summary>Приложение №1: текст для вставки в файл README.md</summary>

Мы на столько крутые, что уже успели поработать со следующими команиями:

1. ООО «Рога и копыта»
2. Издательство «Читый лист»
3. Космопорт «Черезтерновый Кзвёздный»
4. Дизайн-студия имени Слишком Известного Персонажа

Ниже пример кода из нашего приложения:

```css
.selector {
  font-family: "Awesome", Arial, sans-serif;
  color: red;
}
```

</details>

### Задача

1. Найдите ваш репозиторий, созданный для [задачи №1 «Демонстрация»](../introduction#задача-1---демонстрация) к предыдущей лекции. Все дальнейшие шаги следует выполнять в нём;
1. Создайте ветку **feature/code-documentation** и переключитесь на неё;
1. Вставьте текст из **Приложения №1** (находится над заголовком «Задача») в файл `README.md` ниже того текста, что там уже есть. Для блока кода используйте три бэктика и `css` в качестве технологии.
1. Создайте отдельный репозиторий на GitHub'е;
1. Свяжите ваш локальный репозиторий с только что созданным удалённым репозиторием. При связывании используйте _кодовое имя_ `target`.
1. Отправьте в удалённый репозиторий произведённые изменения;
1. Переключитесь на ветку `master` (или `main`) и отправьте её в удалённый репозиторий;
1. Убедитесь, что ветка **feature/code-documentation** попала на GitHub. В итоге в вашем проекте должно получиться две ветки.

**В качестве результата пришлите проверяющему ссылку на ваш репозиторий на GitHub**

## Задача №2 - Слияние изменений

### Легенда

Поскольку разработка новых функций в ветках — ключевой подход при работе с Git'ом, то ваши коллеги также разрабатывают функции в новых ветках. Один из ваших коллег попросил помочь ему со слиянием тех изменений, которые он сделал. Помогите ему.

### Задача

1. Клонируйте Git-репозиторий [по ссылке](https://github.com/netology-code/git-homeworks-neuro-merge/tree/master);
1. Слейте ветку **origin/feature/earlyorder** с веткой **main** 
1. Разрешите появившийся при слиянии конфликт;
1. Создайте отдельный репозиторий на GitHub'е;
1. Свяжите ваш локальный репозиторий с только что созданным удалённым репозиторием. При связывании используйте _кодовое имя_ `target`.
1. Отправьте локальные изменения ветки `main` в удалённый новый репозиторий `target`.

**В качестве результата пришлите проверяющему ссылку на ваш репозиторий на GitHub**


#### Справка: Клонирование

Посмотреть все ветки, включая удалённые, вы можете командой: `git branch -a`.

## Задача №3 - Работа с историей и переключение между коммитами

### Легенда

Проект NeuroStartUp всё больше развивается и всё больше разработчиков подключается к проекту. Лендинг постоянно оптимизируется под маркетинговые кампании и запросы. Но тут выясняется, что перестала работать функция «Подписаться на новости», а это достаточно важная функция. Вы знаете лишь, что всё работало в коммите `c2e06a`, а когда перестало работать - никто не знает.

Вам нужно найти в каком из коммитов функция сломалась и кто её сломал (чтобы он потом починил :smiley:).

### Задача

1. Клонируйте Git-репозиторий [по ссылке](https://github.com/netology-code/git-homeworks-neuro-broken);
1. Переключитесь на коммит `c2e06a`, удостоверьтесь, что функция работает*;
1. Переключитесь на последний коммит;
1. Используя команды переключения между коммитами, определите в каком коммите и кем была внесена ошибка. После переключения между коммитами обновляйте открытый в браузере файл `index.html`.

**Примечание**:\* чтобы проверить, что функция работает, нужно открыть в браузере файл `index.html` (просто два раза кликните на этом файле в файловом менеджере), ввести в поле ввода подписки адрес электронной почты и нажать кнопку. В коммите `c2e06a` форма работает, после отправки формы появляется окошко с текстом.

Окошко с текстом будет выглядеть примерно вот так (если у вас тёмная тема оформления браузера):
![](pic/alert.png)

**В качестве результата пришлите Имя автора и идентификатор первого коммита, в котором функция перестала работать. Вставьте ответ в поле "Комментарий". Не прикладывайте файлы к решению**

-----------

Все задачи обязательны к выполнению. Присылать на проверку можно только сразу все три задачи.

Любые вопросы по решению задач задавайте в канале курса в Slack.
```