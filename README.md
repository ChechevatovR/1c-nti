# Система автоматизации приемной кампании

В этом репозитории хранится решения задачи 
заключительного этапа школьного трека Олимпиады КД НТИ по профилю 
Автоматизация бизнес-процессов 2021 года.

К сожалению, условие задачи утеряно, 
но как часть решения нами была создана сопроводительная записка,
подробно описывающая функционал системы.
Кроме самой системы, задание также требовало составить несколько диаграмм,
описывающих работу системы.
Эти диаграммы так же приложены.

Решением задачи является информационная база для платформы
1С Предприятие 8. 
Для запуска необходимо установить Платформу,
открыть информационную базу, указав путь к папке `infobase`.
Или же создать нонвую, потом загрузить информационную базу из выгрузки
(файл `solution.dt`) по представленной в разделе 0 инструкции.

Однако, прошу заметить, что согласно требованию задачи, 
пользователи системы должны проходить авторизацию
с использованием возможностей платформы 1С предприятие.
В доступной бесплатно учебной версии платформы этот функционал 
ограничен - доступна только авторизация без пароля.
Для всех созданных учетных записей пароль был убран: информация
в пояснительной записке касательно паролей неактуальна.

Предоставленное здесь решение создано командой из двух человек в течение
5 дней.

Задача публиковалась постепенно в течение 4 или 5 дней, решение
отправлялось и проверялось также каждый день.

## Восстановленное по памяти условие задачи

Требуется создать систему автоматизации работы приемной комиссии 
Сызранского Государственного Университета 
(вымышленная авторами задачи организация).

Должен быть реализован интерфейс абитуриента с возможностью регистрации.
После регистрации абитуриент может заполнить анкету, указав свои данные
и приложив необходимые документы.
Абитуриенту должны быть доступны рейтинговые таблицы для оценки своих
шансов на поступление.
Подробные требования к прилагаемым документам и полям анкеты были указаны
в задании.
Шаблоны документов которые необходимо печатать должны формироваться
системой автоматически.
Личный кабинет абитуриента также доступен через веб-интерфейс,
но предварительно необходимо установить веб-сервер (например Apache) и 
сконфигурировать для работы с 1С.

Сотрудник приемной комиссии должен иметь возможность просматривать список
абитуриентов и их анкеты.
Полностью заполненные анкеты могут быть проверены сотрудником, и либо
отправлены на доработку с указанием недочетов, либо приняты.
В обоих случаях абитуриент должен получить информативное письмо на 
электронную почту.

Сотрудник приемной комиссии может сформировать приказ о зачислении абитуриентов
(формирование не является вступлением в силу, а лишь "чтобы посмотреть").
После этого студентам автоматически назначается номер группыб формируются документы
(зачетная книжка, читательский билет, ...) по описанным в задании правилам и шаблонам.

Сотрудник деканата факультета видит список студентов своего факультета,
может изучать личное дело, выставлять оценки.

Студенту в информационной системе доступна информация о своих оценках,
о расписании, личное дело.