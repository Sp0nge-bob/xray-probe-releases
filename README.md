# Xray Probe Releases

Публичные APK и манифест самообновления Xray Probe / CaelixFlow.

## Последняя версия: 0.6.0

- [Скачать XrayProbe-0.6.0.apk](https://github.com/Sp0nge-bob/xray-probe-releases/releases/download/v0.6.0/XrayProbe-0.6.0.apk)
- [Последний APK](https://github.com/Sp0nge-bob/xray-probe-releases/releases/latest/download/XrayProbe-latest.apk)
- [Описание релиза](https://github.com/Sp0nge-bob/xray-probe-releases/releases/tag/v0.6.0)
- [Манифест самообновления](https://raw.githubusercontent.com/Sp0nge-bob/xray-probe-releases/main/version.json)

Android 8.0+ (API 26), ARM64. versionCode **11**, размер **14 279 506 байт**.

SHA-256 APK: `f715d08f8e661128b58e3758175bad0c05aa72f22f92feb9ad900d053872a21a`.

## Возможности

- **Симуляционный стенд iOS NetworkExtension & LibXray**: проверка совместимости подписок и конфигураций с iPhone непосредственно на Android без системного VPN.
- **L3 tun2socks Go bridge (`libtun2socks.so`)**: трансляция L3 IPv4 пакетов в SOCKS5 UDP Associate (:53) и TCP CONNECT (окно 65535, эквивалент `NEPacketTunnelFlow`).
- **Универсальный декодер (`SubscriptionDecoder`)**: парсинг Xray JSON, `subscription.raw`, URI `vless://`, `vmess://`, `trojan://`, `ss://` и base64 списков.
- **Apple Jetsam Watchdog**: мониторинг RSS памяти ядра Xray (`/proc/<pid>/statm`) с порогом 50 МБ и опциональным strict kill при превышении.
- **Сквозное тестирование**: L3 DNS UDP :53 (проверка A/AAAA) + L3 TCP HTTP GET (замер TTFB и заголовков).
- **Интеграция в UI и API**: нативная карточка стенда с индикатором памяти Jetsam, endpoint `POST /ios/test`, команда CLI `node client.cjs ios-test`.
- **Выбор ядер Xray-core**: выбор последних 10 официальных релизов Xray-core, динамическое скачивание и проверка SHA-256 до распаковки.
- Встроенное Xray-core **26.9.9**, диагностический Termux loopback API, раздельные UID Probe/Termux.

## Единый ключ подписи

0.6.0 в приватном и публичном репозиториях подписан единым ключом ПК из GitHub Actions CI.

SHA-256 сертификата: `4774185f2c532b0cf5b7d6825f648530c8c24829a5fab6ed4c32d3d7ff402c21`.

Все дальнейшие сборки ПК/Termux/CI используют этот ключ. Старые APK со старыми сертификатами (до 0.5.4) не совместимы для обновления поверх; установку выполняет пользователь. Ключ и пароль не публикуются.

## Проверки

Host unit tests (`HelperTests.java`, `DownloadTests.java`), APK v2/v3 signatures, privacy scans без находок.
