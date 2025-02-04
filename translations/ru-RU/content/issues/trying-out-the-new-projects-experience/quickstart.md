---
title: Краткое руководство по проектам (бета-версия)
intro: Повысьте скорость, гибкость и настройку проектов (бета-версии) путем создания проекта в этом интерактивном руководстве.
allowTitleToDifferFromFilename: true
miniTocMaxHeadingLevel: 3
versions:
  fpt: '*'
  ghec: '*'
type: quick_start
topics:
- Projects
ms.openlocfilehash: 3baf341d38b59e20e6fe1e677e338d6bec1d57da
ms.sourcegitcommit: 22d665055b1bee7a5df630385e734e3a149fc720
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "145135317"
---
{% data reusables.projects.projects-beta %}

## <a name="introduction"></a>Введение

В этом руководстве показано, как применять проекты (бета-версия) для планирования и отслеживания работ. В этом руководстве вы создадите новый проект и добавите настраиваемое поле для отслеживания приоритетов задач. Вы также узнаете, как создавать сохраненные представления, которые помогают обмениваться приоритетами и прогрессом с участниками совместной работы.

## <a name="prerequisites"></a>Предварительные требования

Вы можете создать проект организации или проект пользователя. Чтобы создать проект организации, вам потребуется организация {% data variables.product.prodname_dotcom %}. Дополнительные сведения о создании организации см. в разделе [Creating a new organization from scratch](/organizations/collaborating-with-groups-in-organizations/creating-a-new-organization-from-scratch) (Создание новой организации с нуля).

В этом руководстве вы добавите в новый проект существующие проблемы из репозиториев, принадлежащих организации (для проектов организации) или вам лично (для проектов пользователя). Дополнительные сведения о создании проблем см. в [этом разделе](/issues/tracking-your-work-with-issues/creating-an-issue).

## <a name="creating-a-project"></a>Создание проекта

Для начала создайте проект организации или проект пользователя.

### <a name="creating-an-organization-project"></a>Создание проекта организации

{% data reusables.projects.create-project %}

### <a name="creating-a-user-project"></a>Создание проекта пользователя

{% data reusables.projects.create-user-project %}

## <a name="setting-your-project-description-and-readme"></a>Настройка описания проекта и файла README

{% data reusables.projects.project-description %}

## <a name="adding-issues-to-your-project"></a>Добавление проблем в проект

Затем добавьте в проект несколько проблем.

При инициализации нового проекта вам будет предложено добавить в него элементы. Если вы потеряете это представление или позже решите добавить дополнительные проблемы, поместите курсор в нижнюю строку проекта рядом со значком {% octicon "plus" aria-label="plus icon" %}.

1. Введите `#`.
2. Выберите репозиторий, в котором находится проблема. Чтобы сузить параметры поиска, можно начать вводить часть имени этого репозитория.
3. Выберите проблему. Чтобы снизить количество вариантов, можно ввести часть заголовка проблемы.

Чтобы добавить в проект несколько проблем, повторите эти действия несколько раз.

Дополнительные сведения о других способах добавления проблем в проект и о других элементах, которые можно добавить в проект, см. в статье [Создание проекта](/issues/trying-out-the-new-projects-experience/creating-a-project#adding-items-to-your-project).

## <a name="adding-draft-issues-to-your-project"></a>Добавление черновиков проблем в проект

Теперь добавьте в проект черновик проблемы

1. Установите курсор в нижнюю строку проекта рядом с {% octicon "plus" aria-label="plus icon" %}.
1. Введите идею и нажмите клавишу **ВВОД**.
1. Щелкните заголовок черновика проблемы. В появившемся поле ввода с разметкой Markdown введите дополнительные сведения о проблеме и щелкните **Сохранить**.

## <a name="creating-a-field-to-track-priority"></a>Создание поля для отслеживания приоритета

Теперь создайте настраиваемое поле с именем `Priority` для хранения значений `High`, `Medium`или `Low`.

1. {% data reusables.projects.open-command-palette %}
2. Начните вводить любую часть фразы "Создать новое поле".
3. Выберите **Создать новое поле**.
4. Во всплывающем окне введите в текстовое поле `Priority`.
5. В раскрывающемся списке выберите **Единичный выбор**.
6. Добавьте параметры для `High`, `Medium` и `Low`. В параметры также можно включать эмодзи.
   ![Пример нового поля единичного выбора](/assets/images/help/projects/new-single-select-field.png)
7. Выберите команду **Сохранить**.

Укажите приоритет для всех проблем в проекте.

![Примеры приоритетов](/assets/images/help/projects/priority_example.png)

## <a name="grouping-issues-by-priority"></a>Группирование проблем по приоритету

Затем сгруппируйте все элементы проекта по приоритетам, чтобы упростить обзор элементов с высоким приоритетом.

1. {% data reusables.projects.open-command-palette %}
2. Начните вводить любую часть фразы "Группировать по".
3. Выберите **Группировать по: приоритет**.

Чтобы изменить приоритет проблемы, переместите ее в другую группу.

1. Выберите проблему.
2. Перетащите ее в другую группу приоритета. При этом приоритет проблемы изменится в соответствии с новой группой.

![Перемещение проблемы между группами](/assets/images/help/projects/move_between_group.gif)

## <a name="saving-the-priority-view"></a>Сохранение представления приоритета

Когда вы на предыдущем шаге сгруппировали проблемы по приоритету, в проекте отобразился индикатор, наличия изменений в представлении. Сохраните эти изменения, чтобы все участники совместной работы видели задачи, сгруппированные по приоритету.

1. Нажмите на раскрывающееся меню рядом с именем представления.
2. Нажмите кнопку **Сохранить изменения**.

Чтобы указать назначение представления, присвойте ему описательное имя.

1. Поместите курсор в текущее имя представления — **Представление 1**.
2. Замените существующий текст новым именем — `Priorities`.

Вы можете передать этот URL-адрес другим сотрудникам, чтобы все были в курсе приоритетов по проекту.

После сохранения представления его будет видеть каждый, кто открывает этот проект. В нашем упражнении вы выполнили группировку по приоритетам, но здесь можно добавить и другие модификаторы, такие как сортировка, фильтр или макет. Теперь вы создадите новое представление с измененным макетом.

## <a name="adding-a-board-layout"></a>Добавление макета доски

Чтобы проверить ход выполнения проблем по проекту, переключитесь на макет доски.

Макет доски основан на поле состояния, поэтому для каждой проблемы в проекте нужно указать состояние.

![Пример состояния](/assets/images/help/projects/status_example.png)

Теперь создайте новое представление.

1. Щелкните {% octicon "plus" aria-label="the plus icon" %} **Новое представление** рядом с самым правым представлением.

Затем перейдите к макету доски.

1. {% data reusables.projects.open-command-palette %}
2. Начните вводить любую часть фразы "Переключить макет: Доска".
3. Щелкните **Переключить макет: Доска**.
   ![Примеры приоритетов](/assets/images/help/projects/example_board.png)

Когда вы изменили макет, в проекте отобразился индикатор наличия изменений в представлении. Сохраните это представление, чтобы вы и ваши коллеги могли легко открывать его в будущем.

1. Нажмите на раскрывающееся меню рядом с именем представления.
2. Нажмите кнопку **Сохранить изменения**.

Чтобы указать назначение представления, присвойте ему описательное имя.

1. Поместите курсор в текущее имя представления — **Представление 2**.
2. Замените существующий текст новым именем — `Progress`.

![Примеры приоритетов](/assets/images/help/projects/project-view-switch.gif)

## <a name="configure-built-in-automation"></a>Настройка встроенной автоматизации

Наконец, добавьте встроенный рабочий процесс, чтобы задать состояние **Todo** всем элементам, добавляемым в проект.

1. В проекте выберите {% octicon "workflow" aria-label="the workflow icon" %}.
2. В разделе **Рабочие процессы по умолчанию** щелкните **Элемент, добавленный в проект**.
3. Рядом с пунктом **Когда** должны быть выбраны элементы `issues` и `pull requests`.
4. Рядом с пунктом **Задать** выберите **Состояние:Todo**.
5. Щелкните переключатель **Отключено**, чтобы включить этот рабочий процесс.

## <a name="next-steps"></a>Дальнейшие действия

Проекты можно использовать для широкого спектра задач. Пример:

- отслеживание работы для выпуска;
- планирование спринта;
- определение приоритета невыполненной работы.

Далее приведены некоторые полезные ресурсы для выполнения следующих этапов с помощью {% data variables.product.prodname_github_issues %}.

- Чтобы оставить отзыв о проектах (бета-версия), перейдите в [репозиторий отзывов GitHub](https://github.com/github/feedback/discussions/categories/issues-feedback).
- Дополнительные сведения о том, как проекты помогают в планировании и отслеживании, см. в статье [О проектах](/issues/trying-out-the-new-projects-experience/about-projects).
- Дополнительные сведения о полях и элементах, которые можно добавить в проект, см. в статье [Создание проекта](/issues/trying-out-the-new-projects-experience/creating-a-project).
- Дополнительные сведения о том, как можно отображать необходимые сведения, см. в статье [Настройка представлений проекта](/issues/trying-out-the-new-projects-experience/customizing-your-project-views).
