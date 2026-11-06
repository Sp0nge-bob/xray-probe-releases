# Xray Probe Releases

Публичные APK и манифест самообновления Xray Probe / CaelixFlow.

## Последняя версия: 0.5.4

- [Скачать XrayProbe-0.5.4.apk](https://github.com/Sp0nge-bob/xray-probe-releases/releases/download/v0.5.4/XrayProbe-0.5.4.apk)
- [Последний APK](https://github.com/Sp0nge-bob/xray-probe-releases/releases/latest/download/XrayProbe-latest.apk)
- [Описание релиза](https://github.com/Sp0nge-bob/xray-probe-releases/releases/tag/v0.5.4)
- [Манифест самообновления](https://raw.githubusercontent.com/Sp0nge-bob/xray-probe-releases/main/version.json)

Android 8.0+ (API 26), ARM64. versionCode **10**, размер **13 464 303 байт**.

SHA-256 APK: `93bad2199e7b7ea8105a9b1045a70ad13b48b18de5710cb8c7468f7fecec1b0f`.

## Возможности

- Оформленный выбор последних 10 официальных релизов Xray-core, активное ядро и установленные версии; без ручного ввода версии в UI.
- Смена/загрузка ядра только в простое, общий admission gate UI/API.
- Понятный прогресс ядра и APK: подключение, МБ, проценты, проверка SHA-256.
- Обязательная SHA-256 проверка ядра из официального `.zip.dgst` до распаковки и обязательная проверка APK.
- Увеличенные тайм-ауты GitHub/CLI.
- Встроенное Xray-core **26.9.9**, диагностический Termux loopback API, раздельные UID Probe/Termux без изменения Happ.

## Единый ключ подписи

0.5.4 в приватном и публичном репозиториях — один и тот же проверенный APK из GitHub Actions, подписанный предоставленным ключом ПК.

SHA-256 сертификата: `4774185f2c532b0cf5b7d6825f648530c8c24829a5fab6ed4c32d3d7ff402c21`.

Все дальнейшие сборки ПК/Termux/CI должны использовать этот ключ. Старые APK с другими сертификатами не совместимы для обновления поверх; установку выполняет пользователь. Ключ и пароль не публикуются.

## Проверки

39 Node tests + Java host tests, APK v2/v3 signatures, privacy scans без находок. Это не заменяет проверку интерфейса и загрузки/переключения ядра на Android.
