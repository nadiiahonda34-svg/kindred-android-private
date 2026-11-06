# Исходники Kindred 1.0.35

**Перед загрузкой ZIP проверьте:** этот репозиторий должен быть **Private**, а не Public. Для этого откройте Settings → General → Danger Zone → Change repository visibility → Make private.

После смены видимости откройте папку `android-source`, нажмите **Add file → Upload files**, выберите `Kindred_1_0_35_Unified_Source.zip` и нажмите **Commit changes**. На телефоне при необходимости включите в браузере режим «Версия для ПК».

Для защиты от ошибок workflow проверяет точную контрольную сумму SHA-256 ZIP:
`b279d59f6eec5cfaacaa5991c68ab97f13d8600c876d819f91db90e467c45a23`.

Затем откройте GitHub → **Actions → Kindred 1.0.35 Android build**. Во время сборки будут скачаны SDK Android API 37, Gradle и зависимости, выполнены тесты и сформирован **неподписанный** AAB.

Важно: ключ подписи Google Play **не добавляйте** в GitHub-файлы или переписку. Его можно подключить через GitHub Actions Secrets, отдельно от кода, когда проект успешно соберётся.
