# Лабораторная работа №27. Знакомство с ASP.NET Core: первый веб-сервер на C#

**ФИО**: Пономарёва Наталья Андреевна
**Группа**: ИСП-232
**Дата**: 10.05.2026

## Краткое описание работы

Понять, что
такое HTTP-запрос и HTTP-ответ. Создать минимальный веб-сервер на ASP.NET Core.
Разобраться с маршрутизацией и middleware.

## Структура проекта

+ img - скриншоты
+ Webserver - главная папка проекта
+ README.md - о проекте

|Характеристика|ASP.NET Core|
|-|-|
|Создание сервера|WebApplication.CreateBuilder()|
|Запуск|app.Run()|
|Маршрут GET|app.MapGet("/", fn)|
|Параметр маршрута|{name} → (string name)|
|Возврат JSON |return new {...} / Results.Ok(...)|
|Middleware|app.Use(async (ctx, next) => ...)|
|Логирование|Встроенное + Console.WriteLine|
|Статус ответа|Results.NotFound(...)|
|Тип данных|Строгие (C# record, class)|