В этом репозитории предложены задания для курса по фотограмметрии в [CSCenter](https://compscicenter.ru/courses/photogrammetry/) и [CSClub](https://compsciclub.ru/courses/photogrammetry/).

[Остальные задания](https://github.com/PhotogrammetryCourse/PhotogrammetryTasks2021/).

# Задание 1. Локальные ключевые точки SIFT (детектор и дескриптор)

[![Build Status](https://travis-ci.com/PhotogrammetryCourse/PhotogrammetryTasks2021.svg?branch=task01)](https://travis-ci.com/PhotogrammetryCourse/PhotogrammetryTasks2021)

0. Сделать fork проекта
1. Выполнить задания ниже
2. Отправить **Pull-request** с названием```Task01 <Имя> <Фамилия> <Аффиляция>```:

 - Указав вывод каждой программы при исполнении **на CI** (через редактирование описания PR после того как CI отработает) - в тройных кавычках для сохранения форматирования
 - Перечислив свои мысли по вопросам поднятым в коде и просто появившиеся в процессе выполнения задания (выписывайте их с самого начала в отдельный текстовый файл)

**Дедлайн**: начало лекции 16 февраля.

Если времени не хватит - отправьте то, что вы успели сделать
(и мне очень поможет, если вы сможете детализировать, на чем застряли и на что ушло слишком много времени).

Задание 1.0.
=========

Ознакомьтесь со структурой проекта:

1. ```src/phg/sift/``` - основная часть где вы будете реализовывать алгоритм

2. ```tests/test_sift.cpp``` - тесты которые будут прогонять ваш алгоритм на каких-то относительно простых манипуляциях с маленькой картинкой, если вам хочется добавить другие сценарии тестирования (возможно с другими метриками) - здорово!

3. ```data/src``` - исходные данные используемые при тестировании (к ним используются относительные пути, поэтому нужно выставить Working directory = путь к проекту)

4. ```data/debug/test_sift/SIFT``` - сюда тесты сохранят картинки с визуализацией результата

5. ```data/debug/test_sift/debug``` - сюда вам предлагается сохранять любые промежуточные картинки-визуализации, это очень полезно для отладки, оценки качества, уверенности и в целом один из немногих способов качественно "заглянуть в черную коробку"

Задание 1.1.
=========

Убедитесь что у вас все компилируется и тесты проходят.

Задание 1.2.
=========

Реализуйте SIFT в ```src/phg/sift/sift.cpp```.
