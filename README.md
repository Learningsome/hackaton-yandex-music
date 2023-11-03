# Проект команды "17 мгновений весны", Хакатон "Практикум x Яндекс.Музыка"Я

![Иллюстрация к проекту](https://yielding-character-d3f.notion.site/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F2baaeed3-17c9-4763-bd41-59890c1e9406%2F78607ed7-bcb2-484b-92eb-0630853cb3c4%2F2023-10-20_09.47.37.jpg?table=block&id=ccfa20ce-dc10-4ef5-9e37-e73aa09dfc3f&spaceId=2baaeed3-17c9-4763-bd41-59890c1e9406&width=2000&userId=&cache=v2)



## Участники команды
- [Mikhalchuk Yana](https://github.com/YanaMikhalchuk) (Project Manager)
- [Koptsev Andrei](https://github.com/AVKopt) (Data Science)
- [Nikiforova Ksenia](https://github.com/nikiforovaks) (Data Science)
- [Kashirskii Nikolai](https://github.com/Learningsome) (Data Science)

## Над чем работали
При работе над проектом мы придерживались функционального подхода к решению задач. Все функции содержат докстрингу, которая описывает суть функции, входные параметры, возвращаемые значения и комментарии к коду, где это необходимо.

Разработали ML-модель для сопоставления текстов музыкальных произведений и для поиска каверов (вариации обработки оригинала с элементами новой аранжировки) по их текстам.  

*Задачи, которые были решены*:
- [x] Классификация треков по признаку кавер-некавер; 
- [x] Группировка каверов и исходного трека.

## Используемый стек технологий:
Pandas, numpy, scikit-learn, torch, lightgbm, sentence-transformers, langdetect, pandarallel, requests, joblib, pillow, musicbrainzngs, lyricsgenius, matplotlib, seaborn, colorama.

Более подробную информацию о стеке и зависимостях описали в файле [requirements.txt](https://github.com/Learningsome/hackaton-yandex-music/blob/main/requirements.txt)

## Структура проекта
Исследования проводились каждым участником в своей папке репозитория (папки названы по ФИО участника).

Решение:
Подробное решение описано в папке [solutiion](https://github.com/Learningsome/hackaton-yandex-music/tree/main/solution), в которой находятся 4 тетрадки, каждая из которых выполняет свою функцию:
- [Парсинг данных](https://github.com/Learningsome/hackaton-yandex-music/blob/main/solution/01-text-parsing.ipynb)
- [Предварительная обработка данных](https://github.com/Learningsome/hackaton-yandex-music/blob/main/solution/02-data-preprocessing.ipynb)
- [Кодирование текстов песен в эмбеддинги](https://github.com/Learningsome/hackaton-yandex-music/blob/main/solution/03-text-encoding.ipynb)
- [Классификация треков + группировка каверов и исходных треков](https://github.com/Learningsome/hackaton-yandex-music/blob/main/solution/04-tracks-classification-and-grouping.ipynb)

## Вывод
В результате исследования были построены 2 модели:

- модель классификации,
- модель нахождения кавер-треков и/или исходников к заданному треку в датасете.

Классификация проводилась на основе метаданных. 
Модель нахождения кавер-треков и/или исходников к заданному треку находит заданный трек и выводит список нужных треков.


