# Аналитическая лабораторная. AWS.
## Команда Вуха:
* Калачева Вера К3223
* Петрова Виктория К3223
* Денисов Илья К3223
* Марков Даниил К3223
  
## Цель работы: 
Знакомство с облачными сервисами. Понимание уровней абстракции над инфраструктурой в облаке. Формирование понимания типов потребления сервисов в сервисной-модели. Сопоставление сервисов между разными провайдерами. Оценка возможностей миграции на отечественные сервисы.

## Дано:
1. Слепок данных биллинга от провайдера после небольшой обработки в виде SQL-параметров. Символ % в начале/конце означает, что перед/после него может стоять любой набор символов.
2. Google с документациями провайдера.

## Параметры классификации сервисов
1. **IT Tower** - технологическая область или область обслуживания:
    - Data Center 
    - Compute
    - Storage
    - Network 
    - Platform
    - Output 
    - End User
    - Application
    - Delivery 
    - Security 
    - IT Management
    - и т.д.
2. **Service Family** - категория сервисов, выполняющих конкретную задачу:
    - Infrastructure Services
    - Application Services
    - End-User Services
    - Cloud Services
    - Security Services
    - и т.д.
3. **Service Type** - тип сервиса:
    - Data Security Service
    - Machine learning service
    - Cloud storage
    - и т.д.
4. **Service Usage Type** - тип использования сервиса

## Заполненная таблица
![/AWS vukha table1.jpg](https://github.com/verkalacheva/aws_vukha/blob/main/table%201.jpg)
![/AWS vukha table1.jpg](https://github.com/verkalacheva/aws_vukha/blob/main/table%202.jpg)
## Описание сервисов AWS
| Сервис                                   | Описание                                                                                                                                                                                                                                                                                                                                         |
|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| AmazonMacie                              | Служба безопасности данных, которая обнаруживает конфиденциальные данные с помощью машинного обучения и сопоставления шаблонов, обеспечивает видимость рисков безопасности данных и автоматическую защиту от этих рисков.                                                                                                                    |
| AmazonMSK                                | Полностью управляемый сервис, позволяющий создавать и запускать приложения, использующие Apache Kafka для обработки потоковых данных.                                                                                                                                                                                                            |
| AmazonPolly                              | Облачный сервис, который преобразует текст в реалистичную речь.                                                                                                                                                                                                                                                                              |
| AmazonPersonalize                        | Полностью управляемый сервис машинного обучения, который использует данные для создания рекомендаций по товарам для пользователей. Он также может генерировать пользовательские сегменты на основе привязанности пользователей к определенным товарам или метаданным товаров.                                                     |
| Amazon S3 / Подвид S3 Glacier | Amazon S3 - объектное хранилище, рассчитанное на хранение и извлечение любых объемов данных из любой точки сети. / Подвид S3 Glacier — это сервис для архивирования данных и долгосрочного резервного копирования с использованием хранилищ.                                                                                                                                                                                                                                         |
| Amazon Elasticsearch Service (Amazon ES) | Управляемый сервис, который упрощает развертывание, эксплуатацию и масштабирование Elasticsearch в облаке AWS. Elasticsearch - популярная поисковая и аналитическая система с открытым исходным кодом для таких вариантов использования, как аналитика журналов, мониторинг приложений в режиме реального времени и аналитика потока кликов. |

## Российские аналоги
1. **Сервис Yandex Identity and Access Management (IAM)** — сервис идентификации и контроля доступа, который помогает централизованно управлять правами доступа пользователей к  ресурсам Yandex Cloud. Сервис IAM контролирует доступ к ресурсам и предоставляет функциональность для настройки прав доступа.

Задачи:
* предоставление доступа к ресурсам;
* управление аккаунтами в Yandex Cloud;
* управление ключами для авторизации;
* авторизация в Yandex Cloud.

2. **Сервис Yandex Managed Service for Apache Kafka®** помогает разворачивать и поддерживать кластеры серверов Apache Kafka® версий в инфраструктуре Yandex Cloud.

3. **Yandex SpeechKit** может распознавать речь в режиме реального времени и из предварительно записанных аудиофайлов, автоматически определяя язык говорящего, а также озвучивать шаблонные фразы и развернутые тексты при помощи стандартных голосов SpeechKit. Работает через интерфейсы API.

4. **Облачное объектное хранилище S3 (Selectel)** - сервис Selectel для хранения и раздачи неограниченного объема неструктурированных и полуструктурированных данных.

Задачи: 
* раздача статической информации (данных сайтов и приложений) и потоковая передача данных и т. д.;
* хранение резервных копий и архивов. Вы можете настроить резервное копирование сервера по расписанию, чтобы переносить важные данные в хранилище;
* хранение больших объемов данных для машинного обучения и аналитики;
* размещение статических сайтов.

5. **Yandex Object Storage** позволяет:
* хранить данные произвольного формата как объекты с доступом по текстовому идентификатору;
* использовать различные классы хранилища для объектов и управлять их жизненным циклом;
* хранить большие объекты размером в несколько терабайт;
* опубликовать статический веб-сайт.
  
6. **Сервис Yandex Data Transfer** предназначен для логического переноса данных между источниками и приемниками. В качестве источников и приемников данных могут выступать СУБД, объектные хранилища или брокеры сообщений.

Yandex Data Transfer позволяет:
* переносить  базы данных в облако — как в сервисы управляемых баз данных, так и в собственные инсталляции на базе ВМ Yandex Compute Cloud;
* создавать удаленные реплики баз данных;
* агрегировать данные из разных источников в едином хранилище данных (Data Warehouse) на базе ClickHouse;
* резервировать и сохранять данные из любых доступных источников в Yandex Object Storage;
* сохранять в облачные хранилища произвольные данные, которые поступают от брокеров сообщений.

7. **Yandex Managed Service for Elasticsearch** помогает разворачивать и поддерживать кластеры серверов Elasticsearch в инфраструктуре Yandex Cloud. Сервис позволяет в несколько кликов увеличить или уменьшить потребление облачных ресурсов при изменениях нагрузки. Также Еlasticsearch предоставляет набор аналитических инструментов, с помощью которых можно получать информацию и принимать решения на основе журналов событий и метрик, повышать эффективность операций в ИТ, сокращать время принятия решений, получать данные для разработки и информационной безопасности.
   
## Итоговая таблица
| AWS                                      | Analog                                     |
|------------------------------------------|--------------------------------------------|
| AmazonMacie                              | Yandex Identity and Access Management (IAM)|
| AmazonMSK                                | Yandex Managed Service for Apache Kafka®   |
| AmazonPolly                              | Yandex SpeechKit                           |
| AmazonPersonalize                        |                                            |
| Amazon S3                                | Облачное объектное хранилище S3 (Selectel), Yandex Object Storage, Yandex Data Transfer |
| Amazon Elasticsearch Service (Amazon ES) | Yandex Managed Service for Elasticsearch   |
