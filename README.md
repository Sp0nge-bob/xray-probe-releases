# Xray Probe Releases

Официальный репозиторий публичных релизов и обновлений Android-приложения **Xray Probe** (компонент экосистемы CaelixFlow).

---

## 📥 Последняя версия: v0.5.2

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
Все сборки подписываются официальным release-ключом CaelixFlow. Проверяйте контрольную сумму SHA-256 перед установкой.
