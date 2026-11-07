# FlowZapret components

Подписанный манифест обновляемых компонентов для
[FlowZapret](https://github.com/Steellwolf56/flowzapret).

Этот репозиторий — раздача артефактов, а не исходники. Файлы собираются
скриптом `tools/build-components.sh` и публикуются `tools/publish-components.sh`.

## Файлы

| Файл | Назначение |
| --- | --- |
| `components.json` | манифест обновлений (версии, URL, SHA-256, размеры) |
| `components.json.sig` | подпись манифеста (ECDSA P-256 / SHA-256, base64 DER) |
| `libbyedpi-*.so` | ядро ByeByeDPI + JNI-шимы для `arm64-v8a` / `armeabi-v7a` |
| `libtgwsproxy-*.so` | ядро Telegram MTProto прокси для `arm64-v8a` / `armeabi-v7a` |
| `flowseal_presets.json` | пресеты Flowseal |

## Источник в приложении

```
https://raw.githubusercontent.com/Steellwolf56/flowzapret-components/main/components.json
```

Это значение используется по умолчанию (**меню → Компоненты → Источник обновлений**).

## Лицензия

Артефакты распространяются на условиях **GPL-3.0** в составе FlowZapret.
Источники: [ByeDPI](https://github.com/hufrea/byedpi),
[ByeByeDPI](https://github.com/romanvht/ByeDPIAndroid),
[Flowseal/tg-ws-proxy](https://github.com/Flowseal/tg-ws-proxy).
