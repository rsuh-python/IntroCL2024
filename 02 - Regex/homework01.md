## Домашняя работа 1. 

Каждое задание оценивается от 0 до 10 баллов. 

### Задание 1. 

У нас есть текст:

```
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a hobbit-hole, and that 
means comfort. 
It had a perfectly round door like a porthole, painted green, with a shiny yellow brass knob in the exact middle. The door opened on to a tube-shaped hall like a tunnel: a very comfortable tunnel without smoke, with panelled walls, and floors tiled and carpeted, provided with polished chairs, and lots and lots of pegs for hats and coats - the hobbit was fond of visitors. The tunnel wound on and on, going fairly but not quite straight into the side of the hill - The Hill, as all the people for many miles round called it - and many little round doors opened out of it, first on one side and then on another. 
No going upstairs for the hobbit: bedrooms, bathrooms, cellars, pantries (lots of these), wardrobes (he had whole 
rooms devoted to clothes), kitchens, dining-rooms, all were on the same floor, and indeed on the same passage. 
The best rooms were all on the lefthand side (going in), for these were the only ones to have windows, deep-set round windows looking over his garden, and meadows beyond, sloping down to the river. 
```

Соберите BPE-словарь размером не более 400 токенов для него. Можно написать собственный скрипт или использовать готовые, но если используете готовые, я попрошу прокомментировать их работу. 

### Задание 2. 

Посчитайте расстояние Левенштейна для пар слов:

1. программирование - лингвистика
2. levenshtein - einstein

Можно вручную, а можно с помощью скрипта, но в таком случае опять будьте готовы комментировать его работу. 

### Задание 3. 

Напишите следующие регулярные выражения:

1. Для поиска электронной почты. Считаем, что адрес может содержать только латинские буквы, цифры, нижнее подчеркивание и дефис (ну и собачку с точками).
2. Для поиска пути файла в операционной системе UNIX или Windows (посмотрите: у них различающиеся стандарты). Регулярному выражению должно быть все равно, какая операционная система. Путь файла может быть абсолютным или относительным, может начинаться на букву диска. Регулярное выражение должно содержать две группы, в одной должно отлавливаться имя файла, а в другой его расширение. (Считаем, что у файла обязательно есть расширение).
3. Дано предложение:

        ```
        #[[Time: Обычно"обычно:#frequentative_adverbs_adj:FREQUENTATIVE"] [Experiencer_Metaphoric: бюджет"бюджет:бюджет:BUDGET"] [[ко"к:#preposition:PREPOSITION"] [OrderInTimeAndSpace: второму"второй:TWO_ORDINAL"] Object_Situation: чтению "чтение:READING_OF_THE_DRAFT_LAW"] Predicate: готовится"готовить:готовить:PREPAREDNESS" [[DegreeApproximative: непосредственно"непосредственный:DIRECT_OBLIQUE"] [в"в_Prepositional:#preposition:PREPOSITION"] Locative: Думе"дума:дума:DUMA"]#: [[Agent: депутаты"депутат:депутат:DEPUTY"] Specification_Clause: корректируют"корректировать:корректировать:TO_CORRECT" [[Agent: правительственные"правительство:правительство:GOVERNMENT"] Object_Situation: планы"план:план:SCHEDULE_FOR_ACTIVITY"]]].
        ```
    
    В этом предложении каждое слово размечено семантической ролью, лексическим классом и семантическим классом. Роль - то, что идет сразу после квадратной скобки до :, потом идет само слово, потом его лемма, а через двоеточие идут лекс. класс и сем. класс (заглавными буквами). 
    Напишите регулярное выражение, которое будет находить 1) сем. роль 2) словоформу 3) лемму 4) лексический класс 5) семантический класс в пяти группах. 
