# HZ1
## gevent
Это библиотека для организации одновременных вычислений на основе **libev**. **gevent** предоставляет удобный **API** для задач, связанных с одновременной обработкой данных и работой с сетью.
## hadoop
**Hadoop** — проект фонда **Apache Software Foundation**, свободно распространяемый набор утилит, библиотек и фреймворк для разработки и выполнения распределённых программ, работающих на кластерах из сотен и тысяч узлов. Используется для реализации поисковых и контекстных механизмов многих высоконагруженных веб-сайтов, в том числе, для **Yahoo!** и **Facebook**. Разработан на **Java** в рамках вычислительной парадигмы MapReduce, согласно которой приложение разделяется на большое количество одинаковых элементарных заданий, выполнимых на узлах кластера и естественным образом сводимых в конечный результат.

По состоянию на 2014 год, проект состоит из четырёх модулей — **Hadoop Common** (связующее программное обеспечение — набор инфраструктурных программных библиотек и утилит, используемых для других модулей и родственных проектов), **HDFS** (распределённая файловая система), **YARN** (система для планирования заданий и управления кластером) и **Hadoop MapReduce** (платформа программирования и выполнения распределённых **MapReduce**-вычислений), ранее в **Hadoop** входил целый ряд других проектов, ставших самостоятельными в рамках системы проектов **Apache Software Foundation**.

Считается одной из основополагающих технологий «больших данных». Вокруг **Hadoop** образовалась целая экосистема из связанных проектов и технологий, многие из которых развивались изначально в рамках проекта, а впоследствии стали самостоятельными. Со второй половины 2000-х годов идёт процесс активной коммерциализации технологии, несколько компаний строят бизнес целиком на создании коммерческих дистрибутивов **Hadoop** и услуг по технической поддержке экосистемы, а практически все крупные поставщики информационных технологий для организаций в том или ином виде включают **Hadoop** в продуктовые стратегии и линейки решений.
## rabbitMQ
Программный брокер сообщений на основе стандарта **AMQP** — тиражируемое связующее программное обеспечение, ориентированное на обработку сообщений. Создан на основе системы **Open Telecom Platform**, написан на языке **Erlang**, в качестве движка базы данных для хранения сообщений использует **Mnesia**.

Состоит из сервера, библиотек поддержки протоколов **HTTP**, **XMPP** и **STOMP**, клиентских библиотек **AMQP** для **Java** и **.NET Framework** и различных плагинов (таких как плагины для мониторинга и управления через HTTP или веб-интерфейс или плагин **«Shovel»** для передачи сообщений между брокерами). Имеется реализация клиентов для доступа к **RabbitMQ** для целого ряда языков программирования, в том числе для **Perl**, **Python**, **Ruby**, **PHP**. Поддерживается горизонтальное масштабирование для построения кластерных решений.

## Apache Airflow
Свободная платформа, которая используется для построения, выполнения и мониторинга **ETL** (**Extract-Transform-Loading**) процессов на языке **Python**. Основным понятием в **Airflow** является ориентированный ацикличный граф, где вершины графа — конкретные процессы, а ребра графа — поток управления или информации. Процесс может просто вызывать любую **Python** функцию, а может иметь более сложную логику из последовательного вызова нескольких функций в контексте класса. Для наиболее частых операций уже есть множество готовых наработок, которые можно использовать в качестве процессов.
## Kafka
**Apache Kafka** — распределённый программный брокер сообщений, проект с открытым исходным кодом, разрабатываемый в рамках фонда **Apache**. Написан на языке программирования **Scala** и **Java**.

Спроектирован как распределённая, горизонтально масштабируемая система, обеспечивающая наращивание пропускной способности как при росте числа и нагрузки со стороны источников, так и количества систем-подписчиков. Подписчики могут быть объединены в группы. Поддерживается возможность временного хранения данных для последующей пакетной обработки. Одной из особенностей реализации инструмента является применение техники, сходной с журналами транзакций, используемыми в системах управления базами данных.

Изначально разработан компанией **LinkedIn**, исходные коды проекта открыты в начале 2011 года, включение в **Apache Incubator** состоялось 23 октября 2012 года.
## Spark
**Apache Spark** — фреймворк с открытым исходным кодом для реализации распределённой обработки неструктурированных и слабоструктурированных данных, входящий в экосистему проектов **Hadoop**. В отличие от классического обработчика из ядра **Hadoop**, реализующего двухуровневую концепцию **MapReduce** с хранением промежуточных данных на накопителях, **Spark** работает в парадигме резидентных вычислений (англ. **in-memory computing**) — обрабатывает данные в оперативной памяти, благодаря чему позволяет получать значительный выигрыш в скорости работы для некоторых классов задач, в частности, возможность многократного доступа к загруженным в память пользовательским данным делает библиотеку привлекательной для алгоритмов машинного обучения.

Проект предоставляет программные интерфейсы для языков **Java**, **Scala**, **Python**, **R**. Изначально написан на **Scala**, впоследствии добавлена существенная часть кода на **Java** для предоставления возможности написания программ непосредственно на **Java**. Состоит из ядра и нескольких расширений, таких как **Spark SQL** (позволяет выполнять **SQL**-запросы над данными), **Spark Streaming** (надстройка для обработки потоковых данных), **Spark MLlib** (набор библиотек машинного обучения), **GraphX** (предназначено для распределённой обработки графов). Может работать как в среде кластера **Hadoop** под управлением **YARN**, так и без компонентов ядра **Hadoop**, поддерживает несколько распределённых систем хранения — **HDFS**, **OpenStack Swift**, **NoSQL**-СУБД **Cassandra**, **Amazon S3**.

Ключевой автор — румынско-канадский учёный в области информатики Матей Захария (англ. Matei Zaharia), начал работу над проектом в 2009 году, будучи аспирантом Университета Калифорнии в Беркли. В 2010 году проект опубликован под лицензией BSD, в 2013 году передан фонду **Apache** и переведён на лицензию **Apache 2.0**, в 2014 году принят в число проектов верхнего уровня **Apache**.
# Мониторинг
## Munin
Решение для мониторинга небольших сетей.

Сама система состоит из двух независимых частей: сервера (сам munin), устанавливается на одну машину, куда и будут собираться все данные, и небольшого демона munin-node, который устанавливается на машины, которые мы будем мониторить. Сам этот демон представляет собой небольшой **Perl**-скрипт, который слушает 4949 порт с помощью **Net::Server**. При своём запуске он просматривает плагины, установленные в **/etc/munin/plugins** и запоминает их имена. Раз в 5 минут сервер munin подключается ко всем нодам, получает информацию от всех плагинов и сохраняет себе в базы **rrdtool**. Таким образом, для работы **Munin**'а не нужен даже **MySQL**.
## Pingdom
Это шведское программное обеспечение для мониторинга веб-сайтов в качестве сервисной компании, запущенное в Стокгольме и позднее приобретенное в Остине, штат Техас, компанией **SolarWinds**.
# Сеть
## Amazon EC2
**Amazon Elastic Compute Cloud** (**Amazon EC2**) — веб-сервис, который предоставляет вычислительные мощности в облаке. Сервис входит в инфраструктуру **Amazon Web Services**.

Простой веб-интерфейс сервиса позволяет получить доступ к вычислительным мощностям и настроить с минимальными затратами ресурсов. Он предоставляет пользователям полный контроль над вычислительными ресурсами, а также доступную среду для работы. Сервис сокращает время, необходимое для получения и загрузки нового сервера.
## Amazon S3
**Amazon Simple Storage Service** (**Amazon S3**) — онлайновая веб-служба, предлагаемая **Amazon Web Services**, предоставляющая возможность для хранения и получения любого объёма данных, в любое время из любой точки сети, так называемый файловый хостинг. Впервые появилась в марте 2006 года в США и в ноябре 2007 года в Европе.

**Amazon S3** используется многими другими сервисами для хранения и хостинга файлов. Например, сервис хранения и обмена файлов **Dropbox**, веб-сайты **Twitter** и **Woot.com**, загрузчик игры **Minecraft**.
## Amazon CloudFront
Веб-сервис для доставки контента (содержимого). **CloudFront** интегрируется с другими **Amazon Web Services**. Цель сервиса — дать разработчикам и предприятиям простой способ распространять контент для конечных пользователей с минимальными задержками и высокой скоростью передачи данных. Сервис начал работу 18 ноября 2008 г.
## Ha proxy
**HAProxy** — серверное программное обеспечение для обеспечения высокой доступности и балансировки нагрузки для **TCP** и **HTTP**-приложений, посредством распределения входящих запросов на несколько обслуживающих серверов. Программа написана на **C**.

HAProxy используется в ряде высоконагруженных веб-сайтов, включая **Twitter**, **Instagram**, **Github**, **Stack Overflow**, **Reddit**, **Tumblr**, **DeviantArt**, **Avito** и **OpsWorks product** из **Amazon Web Services**, **W3C** (**W3C Validator**), а также является частью облачной платформы **Red Hat OpenShift** и балансировщиком по умолчанию в облачной платформе **OpenStack**.

HAProxy является программой с открытым исходным кодом и распространяется в соответствии с **GNU General Public License** (**GNU GPL v2**).
## Traefik
----------------------------
# Базы данных
## REDIS
**Redis** (от англ. remote dictionary server) — резидентная система управления базами данных класса **NoSQL** с открытым исходным кодом, работающая со структурами данных типа «ключ — значение». Используется как для баз данных, так и для реализации кэшей, брокеров сообщений.

Ориентирована на достижение максимальной производительности на атомарных операциях (заявляется о приблизительно 100 тыс. **SET**- и **GET**-запросов в секунду на **Linux**-сервере начального уровня). Написана на **Си**, интерфейсы доступа созданы для большинства основных языков программирования.

В период 2010—2013 годов разработка системы спонсировалась компанией **VMware**, с мая 2013 года, после реорганизаций в федерации **EMC** — **VMware**, проект передан в **Pivotal**. С июня 2015 года основной спонсор проекта — компания **Redis Labs**, специально основанная для коммерциализации **Redis**, в неё же перешёл основной разработчик продукта — Сальваторе Санфилиппо.
## Memcached
## ClickHouse
## Cassandra
**Apache Cassandra** — распределённая система управления базами данных, относящаяся к классу **NoSQL**-систем и рассчитанная на создание высокомасштабируемых и надёжных хранилищ огромных массивов данных, представленных в виде хэша.

Написана на языке **Java**, реализует распределённую **hash**-систему, сходную с **DynamoDB**, что обеспечивает практически линейную масштабируемость при увеличении объёма данных. Использует модель хранения данных на базе семейства столбцов (**ColumnFamily**), чем отличается от систем, подобных MemcacheDB, которые хранят данные только в связке «ключ — значение», возможностью организовать хранение хэшей с несколькими уровнями вложенности. Относится к категории отказоустойчивых СУБД: помещённые в базу данные автоматически реплицируются на несколько узлов распредёленной сети или даже равномерно распределяются в нескольких дата-центрах, при сбое узла его функции на лету подхватываются другими узлами, добавление новых узлов в кластер и обновление версии **Cassandra** производится на лету, без дополнительного ручного вмешательства и переконфигурации других узлов. Тем не менее настоятельно рекомендуется заново сгенерировать ключи (токены) для каждого узла, включая существующие, чтобы сохранить качество распределения нагрузки. Генерации ключей для существующих узлов можно избежать в случае кратного увеличения количества узлов (в 2 раза, в 3 раза и так далее).
## Apache HBASE
СУБД класса **NoSQL** с открытым исходным кодом, проект экосистемы **Hadoop**. Написана на **Java**; относится к категории «семейство столбцов» (англ. **wide-column store**), многие технические решения переняты из **Google BigTable**. Работает поверх распределенной файловой системы **HDFS** и обеспечивает **BigTable**-подобные возможности для **Hadoop**, то есть обеспечивает отказоустойчивый способ хранения больших объёмов разреженных данных.

Поддержка сжатия, операции в памяти и фильтр Блума для каждого базового столбца реализованы в соответствии с документацией BigTable. Таблицы в HBase могут служить входом и выходом для работы реализации MapReduce в проекте Hadoop, и могут быть получены не только через **Java API**, но и через **API** (**REST**, **Avro**, **Thrift**). Проекты **Phoenix** и **Trafodion** обеспечивают **SQL**-доступ к данным под управлением **HBase**.

Используется для управления данными в ряде крупных проектов, в частности, **Facebook** в период 2010—2018 годов использовал HBase для платформы сообщений (в 2018 году платформа переведена на **MyRocks**), к числу постоянных пользователей также относятся **Adobe**, **StumbleUpon**, **Twitter**, **Yahoo!** (эксплуатирует **HBase**-кластер из 3 тыс. узлов).
# Конфигурация
## terraform
## vaultproject
https://www.vaultproject.io/
## consul
## ansible
## cookiecutter
https://cookiecutter.readthedocs.io/en/1.7.2/
