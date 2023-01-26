# Smart alarm clock

## Что нужно сделать

Реализовать приложение «Умный будильник».

## Функциональные требования:

- Пользователь должен иметь возможность завести будильник на Х часов Y минут после восхода солнца.
  Пример: пользователь заводит будильник на 01:00. Приложение получает данные о времени восхода солнца,
  допустим 05:30, и заводит будильник на 06:30.
- В расчётное время утра устройство должно издать звук будильника.

## Нефункциональные требования:

- Ввод времени будильника произвести в произвольном виде.
- Время восхода солнца получить из часового пояса и даты, расчёт произвести в фоне с помощью WorkManager.
- Показать уведомление о расчётном времени в виде нотификации.
- Получение часового пояса произвести из геолокации или путём ввода от пользователя.
- Звук будильника выбрать на свой вкус.

## Критерии приёмки:

- Приложение позволяет ввести время будильника.
- Приложение рассчитывает время восхода солнца в фоне из часового пояса и даты.
- Приложение показывает нотификацию с расчётным временем будильника.
- В указанное время приложение издаёт звук будильника.
- Логика расчёта времени будильника покрыта тестами.

---
![Clock](/img/clock.jpg)

## Architecture

- [MVVM](https://ru.wikipedia.org/wiki/Model-View-ViewModel)
- [Clean-Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)
- [Use Case](https://en.wikipedia.org/wiki/Use_case)

## Technologies

- [Jetpack Compose](https://developer.android.com/jetpack/compose)
- [Kotlin](https://kotlinlang.org) - %100 Kotlin
- [Gradle Kotlin DSL](https://docs.gradle.org/current/userguide/kotlin_dsl.html)
- [Coroutines](https://github.com/Kotlin/kotlinx.coroutines) for asynchronous operations
- [Lifecycle-ktx](https://developer.android.com/kotlin/ktx)
- [ViewModel](https://developer.android.com/topic/libraries/architecture/viewmodel)
- [Navigation Component Compose](https://developer.android.com/jetpack/compose/navigation)
- [Dagger Hilt](https://developer.android.com/training/dependency-injection/hilt-android) for Dependency Injection
