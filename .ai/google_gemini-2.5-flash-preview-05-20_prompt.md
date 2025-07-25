**Промт-инструкция для форматирования интервью и создания тематических файлов для Obsidian**

**Цель:** 
Проаналазировать стенограмму. 
Максимально сохранить мысли гостя разбить ее на отдельные тематические файлы в формате Obsidian с использованием внутренних ссылок и обратных ссылок.

**Входные данные:**
*   **Ссылка на YouTube-видео:** [https://www.youtube.com/watch?v=cge2i8XQC_8]
*   Полная стенограмма интервью с таймкодами. Пример формата:
    ```
    [0.0->2.8]  Все решения уже приняты. Жить будем долго, детей будет мало.
    [2.8->6.2]  Собаки. Теперь вы тестируете на них свою вакцину?
    ```

**Шаги выполнения:**

1.  **Предварительная обработка и форматирование основной стенограммы:**
    *   Прочитайте всю предоставленную стенограмму интервью.
    *   Объедините короткие реплики одного спикера, если они следуют друг за другом и относятся к одной мысли.
    *   Сохраните все таймкоды в начале соответствующей реплики.
    *   **Преобразование таймкодов:** Для каждого таймкода в формате `[начало->конец]` используйте значение `начало` (в секундах) для формирования YouTube-ссылки. Например, для `[0.0->2.8]` используйте `0.0` секунд.
    *   **Вставка YouTube-ссылок:** Рядом с каждым таймкодом в стенограмме вставьте кликабельную ссылку на YouTube-видео с соответствующей временной меткой. Формат ссылки: `(https://www.youtube.com/watch?v=VIDEO_ID&t=[секунды]s)`.
    *   Добавьте заголовки или подзаголовки (например, `## [Таймкод] Тема`) для логических блоков беседы, если это возможно, чтобы обозначить смену темы или важный момент.
    *   Сохраните отформатированную стенограмму в файле `Долголетие_v2/formatted-interview-with-timestamps.md`.

2.  **Идентификация ключевых тем и подтем:**
    *   Проанализируйте отформатированную стенограмму и выделите основные темы и подтемы, которые обсуждаются в интервью.
    *   Для каждой темы определите ее название, которое будет использоваться как имя файла и заголовок.
    *   Составьте список всех уникальных тем и подтем.

3.  **Создание отдельных тематических файлов для Obsidian:**
    *   Для каждой идентифицированной темы создайте новый файл в директории `Долголетие_v2/` с именем `[Название Темы].md`.
    *   В каждый тематический файл скопируйте только те фрагменты стенограммы (включая таймкоды и YouTube-ссылки), которые непосредственно относятся к данной теме.
    *   В начале каждого тематического файла добавьте заголовок первого уровня `# [Название Темы]`.
    *   Включите в каждый файл ссылки на другие тематические файлы, если они упоминаются или логически связаны. Используйте формат `[[Название Другой Темы]]`.
    *   В конце каждого тематического файла добавьте раздел "Связанные темы" или "См. также", где будут перечислены ссылки на другие релевантные файлы.

4.  **Создание файла `index.md` (Оглавление):**
    *   Создайте или обновите файл `Долголетие_v2/index.md`.
    *   В этом файле создайте оглавление, содержащее ссылки на все созданные тематические файлы.
    *   Организуйте ссылки по логическим разделам или хронологически, если это применимо. Пример:
        ```markdown
        # Оглавление Интервью

        ## Введение
        * [[Введение в тему]]

        ## Основные Темы
        * [[Биомаркеры старения]]
        * [[Генная терапия]]
        * [[Рапамицин]]
        * [[Образ жизни и питание]]

        ## Заключение
        * [[Будущее долголетия]]
        ```

5.  **Проверка и уточнение:**
    *   Проверьте каждый созданный файл на предмет полноты и точности извлеченной информации.
    *   Убедитесь, что все таймкоды и YouTube-ссылки сохранены.
    *   Проверьте работоспособность всех внутренних ссылок.
    *   Убедитесь, что мысли гостя максимально сохранены и представлены в читабельном виде.
    *   При необходимости, внесите корректировки в названия тем или содержание файлов для лучшей организации.
