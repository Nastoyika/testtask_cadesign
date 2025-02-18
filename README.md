# testtask_cadesign
 Тестовое задание на frontend-разработчика

Проект выполнен в VS Code IDE.
Если он запускается через скачанный репозиторий, то рекомендуется запускать его через VS Code,
с Live Server. 
Запускается Live Server, после чего пользователь автоматически перенаправлен на сайт.
Если проект запускается через Vercel хостинг, то просто перейти по ссылке. Сайт откроется автоматически.

В проекте реализована адаптивная верстка в соответствии с макетом.

Header.
Начиная с 1160 пикселей будет появляться (если равно или меньше этого значения) или 
пропадать (если больше) меню. 
Реализован hover на ссылки (снизу появляется оранжевое подчёркивание). 
Список социальных сетей открывается при наведении курсора на него.
Кнопки в списке меняют цвет при наведении.

Адаптивное меню открывается по кнопке и закрывается также при нажатии на неё 
(или изменении размера экрана больше 1160 пикселей).

Баннер также имеет адаптивную вёрстку. 
При нажатии на кнопку открывается форма для заполнения вакансии.

Список преимуществ реализован с использованием SwiperJS, также как и команда специалистов.

В footer находится вторая кнопка открытия формы заполнения вакансии.

Как действует форма:
1. Большая оранжевая кнопка в верхнем правом углу закрывает форму.
2. Каждый инпут обладает проверкой на введение данных.
Также если пользователь нажал, но ничего не ввёл (на инпуты, что необходимо заполнить),
то отобразиться предупреждение.
Если в имя ввести недопустимый символ, например цифру, то также вылетит предупреждение.
3. В инпуте мобильного телефона была реализована система автоматического приведения к 
формату.
4. Кнопка загрузить резюме отличается по дизайну от вёрстки, но свои функции выполняет.
Файл загружается, отображается его название, а также появляется кнопка "Удалить".
5. Обязательные к заполнению данные помечены *.

Пример вводных данных:
Желаемая вакансия: Программист
Фамилия, имя и отчество: Иванов Иван Иванович (можно поставить цифру, чтобы посмотреть выполнение проверки)
Мобильный телефон: 79005003060 (придуман)
Email - необязательно
Образование: Бакалавриат
Адрес места жительства: Иваново
День рождения: 20.09.1996 (можно ввести как с клавиатуры, так и через календарь)
Загрузить резюме - необязательно
Комментарий - необязательно
Чекбокс - обязательно проставить галку.

После этого кнопка отправить становиться доступной для нажатия. 
При нажатии на неё заполненные данные отправляются в консоль, а инпуты очищаются.