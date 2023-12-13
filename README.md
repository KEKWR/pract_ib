6 вариант

Ссылка на гитхаб программы: 

https://github.com/th3r00t/pyShelf.git

Состав команды и обязанности: 

Зотов Александр Павлович 

Жданов Михаил Юрьевич 

Коткин Артем  Константинович 

Структурные элементы проекта:

Системного программного обеспечения СПО:

Веб-браузеры - позволяют пользователям просматривать и взаимодействовать с блогом.

Базы данных PostgreSQL  - хранят информацию о блоге, пользователях, комментариях и других данных.

Приложения:

PyShelf – основное app.

СУБД – pgAdmin+ PostgreSQL.

Описание ИС:

Информационная система "Библиотека".
Предназначена для учета книг в Библиотеках.

Решаемые бизнес-процессы:

1.	Учет и хранение книг.
2.	Управление складом книг.
3.	Управление выданными книгами и сроками возврата.
Роли пользователей, имеющих доступ к системе:
1. работники библиотекари - основные пользователи системы учет, сохранение, выдача, приём, сортировка книг.
2. администраторы системы - настройка прикладного программного обеспечения и веб-сервера, создание инструкций по пользованию ПО;
3. администраторы СУБД - техническая поддержка БД;
4. администраторы СрЗИ - защита сайта БД, защита от пиратства электронных версий книг;
5. Посетители библиотеки, сайта библиотеки, гости, зарегистрированные пользователи.

Варианты доступа пользователей:

1.	Напрямую – через провод к  серверу.
2.	Через интернет к  сайту и панели администратора.
Инфраструктура:

1.	Веб-сервер (на схеме pyShelf(web));
2.	Корпоративный ПК (на схеме corp PC);
3.	ПК в библиотеке(на схеме Public PC);
4.	кластер серверов БД (на схеме BD).
Каждый тип серверов размещается в своей сетевой зоне (public/inside).

Все сервера под управлением ОС debian, прикладное ПО (приложения) субд - postgres pro, веб сервисы функционируют в docker-контейнерах на базе  apache и nginx.

Средства защиты:

На всех серверах установлен антивирус, ОС сертифицированная, СУБД сертифицированная, прикладное ПО сертифицированное, хэшируется пароль, используются  персональные токены, не  стандартный web порт.





