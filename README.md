# Kindred Android 1.0.35 — сборка

Этот репозиторий предназначен для Android-приложения Kindred и сборки через GitHub Actions.

**Важно:** до загрузки исходников необходимо проверить, что Settings → General → Danger Zone → Change repository visibility показывает **Private**. Сейчас никакие исходники или ключи подписи в репозиторий не загружались.

Сборка: GitHub Actions → Kindred 1.0.35 Android build. После помещения `Kindred_1_0_35_Unified_Source.zip` в папку `android-source/` workflow установит Android SDK API 37, выполнит тесты и соберёт **неподписанный** AAB.

Для обновления Google Play необходим прежний upload key; этот workflow не содержит и не публикует его.

Исходники и подписанные ключи **не следует** загружать в публичный репозиторий.
