# NutriDay — полный Android-проект без ИИ

Проект содержит Android-оболочку на Kotlin и экран приложения в `app/src/main/assets/index.html`.

## Сборка APK на GitHub с телефона

1. Создайте репозиторий GitHub и загрузите **содержимое этой папки** (не только ZIP-файл). В корне репозитория должны быть `settings.gradle`, `build.gradle`, папка `app` и папка `.github`.
2. Откройте вкладку **Actions** в репозитории. Если GitHub попросит включить Actions, разрешите их.
3. Выберите workflow **Build NutriDay APK** и нажмите **Run workflow**. Он также запускается при загрузке/изменении файлов в ветке `main` или `master`.
4. Дождитесь зелёной отметки успешного выполнения. Откройте завершённый запуск и скачайте артефакт **NutriDay-debug-apk**.
5. Распакуйте скачанный артефакт на телефоне и установите `app-debug.apk`. Android может попросить разрешить установку приложений из Chrome/файлового менеджера.

## Состав
- `settings.gradle` — настройки проекта.
- `build.gradle` — версия Android Gradle Plugin.
- `app/build.gradle` — настройки Android-приложения.
- `app/src/main/AndroidManifest.xml` — манифест.
- `app/src/main/java/ru/nutriday/app/MainActivity.kt` — WebView-оболочка.
- `app/src/main/assets/index.html` — интерфейс NutriDay.
- `.github/workflows/android.yml` — автоматическая сборка APK.

ИИ и сервер ИИ не используются. APK debug-сборки предназначен для личной установки и тестирования.
