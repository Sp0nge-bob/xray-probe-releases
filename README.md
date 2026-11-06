# Xray Probe Releases

Официальный репозиторий публичных релизов и обновлений Android-приложения **Xray Probe** (компонент экосистемы CaelixFlow).

---

## 📥 Последняя версия: v0.5.1

- **Файл APK**: [XrayProbe-0.5.1.apk](https://github.com/Sp0nge-bob/xray-probe-releases/releases/download/v0.5.1/XrayProbe-0.5.1.apk)
- **Прямая ссылка на последний релиз**: [XrayProbe-latest.apk](https://github.com/Sp0nge-bob/xray-probe-releases/releases/latest/download/XrayProbe-latest.apk)
- **Манифест обновлений**: [`version.json`](https://raw.githubusercontent.com/Sp0nge-bob/xray-probe-releases/main/version.json)
- **Размер**: ~12.8 МБ (`13 439 727` байт)
- **Минимальная версия Android**: 8.0 (API 26), ARM64
- **SHA-256**: `a3b760c80a7c78531eff36fa5ca76ff1bc6832b6f229c6237aafb79efca0ff9d`

---

## 🚀 Возможности
- **Послойная дифференциальная диагностика L1–L9**: DNS $\rightarrow$ TCP $\rightarrow$ TLS $\rightarrow$ WAF/CDN $\rightarrow$ Nginx $\rightarrow$ WS/XHTTP $\rightarrow$ VLESS.
- **Двухконтурное разделение UID**: прямое сравнение выходного IP приложения (вне VPN) и Termux (внутри Happ).
- **Официальное ядро Xray-core ARM64 v26.9.9** встроено в бинарник.
- **Встроенное самообновление**: проверка актуальной версии и обновление в один клик без сторонних магазинов.

---

## 🔒 Безопасность
Все сборки подписываются официальным release-ключом CaelixFlow. Проверяйте контрольную сумму SHA-256 перед установкой.
