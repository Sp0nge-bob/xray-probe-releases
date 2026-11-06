# Xray Probe Releases

Официальный репозиторий публичных релизов и обновлений Android-приложения **Xray Probe** (компонент экосистемы CaelixFlow).

---

## Предварительный выпуск: v0.5.3

- [APK 0.5.3](https://github.com/Sp0nge-bob/xray-probe-releases/releases/download/v0.5.3/XrayProbe-0.5.3.apk) · [описание и ограничения](https://github.com/Sp0nge-bob/xray-probe-releases/releases/tag/v0.5.3)
- Оформленный выбор последних 10 официальных релизов Xray; idle-only смена ядра; прогресс загрузки ядра/APK; увеличенные тайм-ауты; обязательные SHA-256 проверки.
- SHA-256 APK: `4f46ef9de94ff17fa2045d6355b8231714700000b7dd2a22ebbf74672ed26237` (13 464 303 байт).
- **Подпись отличается от публичной 0.5.2: обновление поверх неё невозможно. Не удаляйте приложение ради обхода ошибки.** Нужен исходный ключ 0.5.2 либо отдельно согласованный план. Сертификат этой сборки: `e7a265900466b423ff93e97fd35324629621c76268bb884510b55e3be57b2a27`.
- До разрешения signing compatibility стабильный `version.json` остаётся на 0.5.2. Это prerelease для отдельной приёмки, не подтверждение проверки на устройстве.

---

## 📥 Последняя стабильная версия: v0.5.2

- **Файл APK**: [XrayProbe-0.5.2.apk](https://github.com/Sp0nge-bob/xray-probe-releases/releases/download/v0.5.2/XrayProbe-0.5.2.apk)
- **Прямая ссылка на последний релиз**: [XrayProbe-latest.apk](https://github.com/Sp0nge-bob/xray-probe-releases/releases/latest/download/XrayProbe-latest.apk)
- **Манифест обновлений**: [`version.json`](https://raw.githubusercontent.com/Sp0nge-bob/xray-probe-releases/main/version.json)
- **Размер**: ~12.8 МБ (`13 456 111` байт)
- **Минимальная версия Android**: 8.0 (API 26), ARM64
- **SHA-256**: `cf1760ff94dca21ac5f5f7c19574a04e4935a11fbdf1401bbd4e671e94ac66b2`

---

## 🚀 Возможности
- **Послойная дифференциальная диагностика L1–L9**: DNS $\rightarrow$ TCP $\rightarrow$ TLS $\rightarrow$ WAF/CDN $\rightarrow$ Nginx $\rightarrow$ WS/XHTTP $\rightarrow$ VLESS.
- **Двухконтурное разделение UID**: прямое сравнение выходного IP приложения (вне VPN) и Termux (внутри Happ).
- **Динамическое ядро Xray-core**: переключение между встроенным ядром v26.9.9 и скачивание любых версий Xray ARM64 с официального GitHub XTLS/Xray-core на лету.
- **Встроенное самообновление**: проверка актуальной версии и обновление в один клик через `ProbeFileProvider` без сторонних маркетов.
- **Termux Loopback API (127.0.0.1:18769)**: управление тестами, ядром (`/xray/*`) и обновлением (`/update/*`) через CLI.

---

## 🔒 Безопасность
Проверяйте SHA-256 APK и совместимость сертификата с установленной сборкой. Публичный APK 0.5.2 имеет сертификат `5ee1b3a71544ea8a33bcdcbd64b48ffa69a002d883852dc1b4cba7ddc9b0ed6c`; prerelease 0.5.3 использует иной существующий локальный сертификат (см. выше). Удаление приложения сбрасывает данные и не является безопасным способом обхода signing mismatch.
