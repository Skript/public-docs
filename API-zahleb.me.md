# API Сайта

## Поиск контента по названию, автору или описанию

GET ```https://zahleb.me/api/search```  

Тело запроса:  
```{ "searchtext":"Title or author or description part" }```

Пример запроса в curl:  
`curl --location --request GET 'https://zahleb.me/api/search' \`  
`--header 'Content-Type: application/json' \`  
`--data-raw '{ "searchtext":"Взахлёб" }'`  

Пример ответа:  
```{
    "result": [
        {
            "storyId": "d2KviLU6G8",
            "textId": "ru-protrendy",
            "title": "Взахлёб. Про тренды.",
            "author": "VZ",
            "subtitle": "Приложение «Взахлёб» уже давно известно своими удивительными и увлекательными историями, а также крутыми аудиоспектаклями. Теперь мы решили попробовать себя ещё и в подкастах. Здесь мы говорим о современных трендах: о популярной музыке, о клипах, о фильмах и сериалах, а ещё о тиктокерах и о ютуберах. Давайте вместе следить за эволюцией нашего подкаста!\n\nПредлагать свои темы нам можно в наших социальных сетях с хештегом #подкаствзахлёб",
            "coverImage": "https://bmap-addicted-stories.eu-central-1.linodeobjects.com/images/protrendy/cover-original.jpg",
            "rating": 4.66666666666667,
            "continued": true,
            "episodesCount": 23,
            "linesCount": 0,
            "hasAudio": true
        }
    ]
}```