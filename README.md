![Логотип ООО ТД Комплект](https://tools.by/themes/tetoo/tdk_logo_h100.jpg) 

# Тестовое задание для web-разработчика Laravel

> Необязательно решить все и правильно. Мы хотим понять, как Вы подходите к решению задач и пишете код. 
Будьте готовы к обсуждению решений на собеседовании, а также к дополнительным задачам.


На выполнение задания отводится **5 дней** с момента получения.

В качестве ответа **не нужно присылать никаких ZIP-архивов и наборов файлов**.
Результат выполнения задания нужно будет оформить на https://github.com/ в вашем публичном репозитории.

Если есть вопросы, вы всегда их можете задать связавшись с человеком, который выдал вам задание.

# Задание: прототип формы анкеты

Представим, что вы работаете в международной компании по продаже автомобилей. 
Для того, чтобы автоматизировать работу своим коллегам, вам предстоит разработать форму,
которая будет контролировать и проверять вводимые данные пользователя перед тем как их сохранить.

## Что необходимо реализовать:
> Требуется реализация графического интерфейса при помощи Livewire
> 
> Сохранение данных в БД

### 1. Форма
Форма должна содержать в себе поля:
- (string) Имя [required] (_лимит макс. кол-во символов определите самостоятельно_)
- (string) Фамилия [required] (_лимит макс. кол-во символов определите самостоятельно_)
- (string) Отчество (_лимит макс. кол-во символов определите самостоятельно_)
- (date) Дата рождения [required]
- (email) Email
- (select) Код страны: +375, +7 && (tel) Телефон (_в международном формате_)
- (select) Семейное положение: Холост/не замужем, Женат/замужем, В разводе, Вдовец/вдова
- (textarea) О себе [max:1000]
- (file) Файлы [max:5|max:5mb|types:jpg,png,pdf|multiple] (_максимально 5 файлов, один файл не должен превышать 5 Мб, разрешенные форматы:jpg,png,pdf_)
- (checkbox) Я ознакомился c правилами [required]
- (button-submit) Отправить [disabled]

### 2. Backend логика
- Форма должна строиться через blade шаблоны Livewire
- Контроллер дополнительно обрабатывает и проверяет данные перед отправкой в БД
- Файлы можно сохранять локально (_важно, как вы их будете хранить в таблице БД_)
- После отправки формы если произошла ошибка на стороне backend, необходимо сохранить введенные данные в полях
- После отправки формы если нет ошибок - записываем данные формы в БД и на этом же экране убираем форму,
вместо нее отображаем результат отправки и текст "Успешно"

### 3. Frontend логика
- Валидация формы и всех ее полей
- Форма не должна отправляться при нажатии на клавишу на клавиатуре Enter (_или на телефоне Ввод_)
- Если все поля заполнены верно - активируем кнопку "Отправить" для возможности отправки формы
- Если поле заполнено не верно - выводим красным текстом под полем ошибку, само поле обводим красной обводкой
- Возле поля "Телефон" должна находится кнопка "+" для добавления дополнительного номера телефона (_добавлять таких полей можно до 5 шт._)
- Поле "Email" и "Телефон" - обязательно должно быть заполнено любое одно (_почта или телефон_) иначе ошибка
- Поле "О себе" можно растянуть только вниз и не более чем на 7 строк

## Дополнительная информация:

- Сервис разрабатывается для "Внутреннего использования"
- Приветствуется наличие документации по первому запуску приложения
- Приветствуется покрытие кода тестами

**Стек:**
- PHP >= 7.3
- MySQL 8
- Laravel >= 9
- Bootstrap 5
- Laravel Livewire

## Обратите внимание

Напомним порядок действий:

1. Мы уже связались с вами, немного пообщались и Вы получили это тестовое задание;
2. Пожалуйста, выполните это тестовое задание и опубликуйте его в своем публичном репозитории на гитхабе;
3. Присылайте ваше решение нашей команде HR (или человеку, который вам высылал это задание);
4. Будьте готовы к обсуждению решений на заключительном/техническом собеседовании.