# Тестовое задание для поступления в GoCloudCamp

## 2. Разработка музыкального плейлиста

### Часть 2: Построение API для музыкального плейлиста

Реализовать сервис, который позволит управлять музыкальным плейлистом. Доступ к сервису должен осуществляться с помощью API, который имеет возможность выполнять CRUD операции с песнями в плейлисте, а также воспроизводить, приостанавливать, переходить к следующему и предыдущему трекам. Конфигурация может храниться в любом источнике данных, будь то файл на диске, либо база данных. Для удобства интеграции с сервисом может быть реализована клиентская библиотека.

### Технические требования

* реализация задания может быть выполнена на любом языке программирования
* сервис должен обеспечивать персистентность данных
* сервис должен поддерживать все CRUD операции
* удалять трек допускается только если он не воспроизводится в данный момент
* API должен иметь необходимые методы для взаимодействия с плейлистом.
* API должен возвращать значимые коды ошибок и сообщения в случае ошибок.


### Будет здорово, если:
* в качестве протокола взаимодействия сервиса с клиентами будете использовать gRPC
* напишите Dockerfile и docker-compose.yml
* покроете проект unit-тестами
* сделаете тестовый пример использования написанного сервиса

### docker-compose
Пример docker-compose.yml с использованием изображения: [docker-compose.yml](https://github.com/Wani4ka/gocloudcamp-web-base/blob/master/docker-compose.yml)

Допускается возможность изменить порт gRPC (параметр `HTTP_PORT` в [.env](https://github.com/Wani4ka/gocloudcamp-web-base/blob/master/.env.example)) и путь к каталогу внутри изображения, в котором будет храниться файл (параметр `STORAGE_PATH` в [.env](https://github.com/Wani4ka/gocloudcamp-web-base/blob/master/.env.example))
