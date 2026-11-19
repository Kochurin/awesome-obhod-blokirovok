<a href="https://kochurin.github.io/blockcheck/"><img src="banner.png" alt="Обход блокировок: всё в одном месте"></a>

# Обход блокировок: всё в одном месте

Подборка на русском: приложения, протоколы, свои серверы, обход DPI, роутеры, прокси для Telegram и гайды. Только проекты, которые живы и обновляются. Список собран автором [SkyrimVPN](https://t.me/SkyrimVPN_bot?start=awesome), наши проекты отмечены ⭐

*Awesome list of censorship circumvention tools, in Russian*

## Содержание

- [Сначала проверьте, что заблокировано](#сначала-проверьте-что-заблокировано)
- [Приложения-клиенты](#приложения-клиенты)
- [Свой VPN-сервер](#свой-vpn-сервер)
- [Ядра и протоколы](#ядра-и-протоколы)
- [Обход DPI без VPN](#обход-dpi-без-vpn)
- [Роутеры](#роутеры)
- [Telegram](#telegram)
- [Списки доменов и правила маршрутизации](#списки-доменов-и-правила-маршрутизации)
- [Гайды](#гайды)
- [Готовые VPN-сервисы](#готовые-vpn-сервисы)

## Сначала проверьте, что заблокировано

- ⭐ [Что у меня заблокировано](https://kochurin.github.io/blockcheck/) — проверка из браузера за несколько секунд: YouTube, Instagram, WhatsApp, Discord, ChatGPT и другие. Удобно сравнить Wi-Fi и мобильный интернет
- [OONI Probe](https://ooni.org/) — приложение для измерения блокировок, результаты попадают в открытую базу ([GitHub](https://github.com/ooni/probe))

## Приложения-клиенты

Подключаются к серверам VLESS, VMess, Trojan, Shadowsocks, Hysteria2 и другим по ссылке или подписке

| Приложение | Платформы | Коротко |
|---|---|---|
| [Happ](https://www.happ.su/) | Android, iOS, Windows, macOS, ТВ | простой клиент, понимает подписки |
| [v2rayNG](https://github.com/2dust/v2rayNG) | Android | классика для Android на ядре Xray |
| [v2rayN](https://github.com/2dust/v2rayN) | Windows, Linux, macOS | клиент для компьютера на Xray и sing-box |
| [Hiddify](https://github.com/hiddify/hiddify-app) | Android, iOS, Windows, macOS, Linux | один клиент на все платформы, ядро sing-box |
| [Karing](https://github.com/KaringX/karing) | Android, iOS, Windows, macOS | поддерживает правила маршрутизации Clash и sing-box |
| [Throne](https://github.com/throneproj/Throne) | Windows, Linux | продолжение NekoRay, который больше не поддерживается |
| Shadowrocket, Stash | iOS, Apple TV | платные, в App Store |

## Свой VPN-сервер

Если есть свой VPS за границей

- [3x-ui](https://github.com/MHSanaei/3x-ui) — веб-панель для Xray: пользователи, лимиты, подписки
- [Marzban](https://github.com/Gozargah/Marzban) — панель для Xray с несколькими протоколами и подписками
- [Hiddify Manager](https://github.com/hiddify/Hiddify-Manager) — панель с установкой в одну команду
- [Amnezia VPN](https://amnezia.org/) — ставит VPN на ваш сервер из приложения, без консоли. Свой протокол AmneziaWG ([клиент](https://github.com/amnezia-vpn/amnezia-client), [AmneziaWG](https://github.com/amnezia-vpn/amneziawg-go))
- [Outline](https://getoutline.org/) — сервер и клиент на Shadowsocks ([сервер](https://github.com/OutlineFoundation/outline-server), [приложения](https://github.com/OutlineFoundation/outline-apps))
- [wg-easy](https://github.com/wg-easy/wg-easy) — WireGuard с веб-панелью. Обычный WireGuard в России часто блокируют, лучше подходит для поездок

## Ядра и протоколы

- [Xray-core](https://github.com/XTLS/Xray-core) — ядро с VLESS и REALITY, на нём работает большинство клиентов
- [sing-box](https://github.com/SagerNet/sing-box) — универсальное ядро, поддерживает почти все протоколы
- [Hysteria](https://github.com/HyNetworks/hysteria) — протокол поверх QUIC, быстрый на плохих сетях
- [v2ray-core](https://github.com/v2fly/v2ray-core) — исходное ядро проекта V2Ray

## Обход DPI без VPN

Не меняют ваш IP, а только мешают оборудованию провайдера распознать трафик. Помогают с замедлением YouTube и Discord, но не с сайтами, заблокированными по IP, и не с белыми списками

- [zapret](https://github.com/bol-van/zapret) — обход DPI для Linux, роутеров и Windows
- [zapret-discord-youtube](https://github.com/Flowseal/zapret-discord-youtube) — готовая сборка zapret для Windows под Discord и YouTube
- [GoodbyeDPI](https://github.com/ValdikSS/GoodbyeDPI) — утилита для Windows
- [ByeDPI](https://github.com/hufrea/byedpi) и [ByeByeDPI](https://github.com/romanvht/ByeByeDPI) — то же для Android, без root
- [SpoofDPI](https://github.com/xvzc/SpoofDPI) — простой обход DPI на Go для macOS и Linux

## Роутеры

VPN на роутере работает для всех устройств дома, включая телевизоры и приставки

- [PassWall 2](https://github.com/Openwrt-Passwall/openwrt-passwall2) — прокси-клиент для OpenWrt
- [Podkop](https://github.com/itdoginfo/podkop) — пускает через VPN только заблокированные сайты, OpenWrt
- ⭐ [SkyrimVPN-Router](https://github.com/Kochurin/SkyrimVPN-Router) — PassWall 2 одной командой и простая панель, российские сайты идут напрямую (бета)

## Telegram

- ⭐ [telegram-mtproto-proxy](https://github.com/Kochurin/telegram-mtproto-proxy) — список живых MTProto-прокси, обновляется каждый час
- [mtg](https://github.com/9seconds/mtg) — свой MTProto-прокси на Go
- [MTProxy](https://github.com/TelegramMessenger/MTProxy) — официальный MTProto-прокси от Telegram
- [mtprotoproxy](https://github.com/alexbers/mtprotoproxy) — MTProto-прокси на Python

## Списки доменов и правила маршрутизации

Чтобы через VPN шли только заблокированные сайты, а российские открывались напрямую

- [allow-domains](https://github.com/itdoginfo/allow-domains) — список заблокированных доменов
- [russia-v2ray-rules-dat](https://github.com/runetfreedom/russia-v2ray-rules-dat) — готовые правила маршрутизации для Xray и v2ray, обновляются сами
- [russia-blocked-geosite](https://github.com/runetfreedom/russia-blocked-geosite) — файлы GeoSite с заблокированными в России сайтами
- [antifilter.download](https://antifilter.download/) — списки заблокированных IP и подсетей

## Гайды

- ⭐ [Белые списки на мобильном интернете: почему не открываются сайты и что делать](https://kochurin.github.io/whitelist-guide/)

## Готовые VPN-сервисы

Если свой сервер не нужен

- ⭐ [SkyrimVPN](https://github.com/Kochurin/SkyrimVPN) — бот в Telegram: VLESS/REALITY и Hysteria2, 50+ серверов в 16 странах, отдельные серверы для мобильного интернета с белыми списками. 3 дня бесплатно ([бот](https://t.me/SkyrimVPN_bot?start=awesome) · [сайт](https://skyrim.connecto.lol/?utm_source=awesome))

## Как добавить проект

Откройте issue или pull request: ссылка, одна строка о том, что делает проект, и для какой платформы. Берём живые проекты с открытым кодом или понятной репутацией

Сеть есть. Интернет тоже
