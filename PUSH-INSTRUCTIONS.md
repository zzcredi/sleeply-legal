# Как опубликовать сайт за 2 минуты

Я сгенерировал готовый сайт в `legal/website/`:
- `index.html` — главная страница со ссылками на 4 документа
- `privacy-policy-en.html` + `privacy-policy-ru.html` — privacy policy на EN и RU
- `terms-of-use-en.html` + `terms-of-use-ru.html` — terms of use на EN и RU
- `.md` файлы — исходники

Тёмная тема, стилизованы под Sleep Architect.

---

## Шаг 1 — Зайти в репозиторий через Terminal

```bash
cd /Users/vladislav/Desktop/SleepArchitect/legal/website
git init
git add .
git -c user.email=zzcredi@gmail.com -c user.name=zcredi commit -m "Initial: privacy policy and terms of use (EN + RU)"
git branch -M main
git remote add origin https://github.com/zcredi/sleeparchitect-legal.git
git push -u origin main
```

При запросе credentials введи свой GitHub username `zcredi` и **Personal Access Token** вместо пароля (на https://github.com/settings/tokens создаётся за 1 минуту).

ИЛИ если GitHub Desktop установлен — просто перетащи папку `legal/website` в его UI и нажми Publish.

---

## Шаг 2 — Включить GitHub Pages

1. https://github.com/zcredi/sleeparchitect-legal/settings/pages
2. Source: **Deploy from a branch**
3. Branch: **main** + folder **/(root)**
4. **Save**
5. Подожди 30-60 секунд (статус обновится сверху страницы)

---

## Шаг 3 — Готовые URL для App Store Connect

После активации Pages твои документы будут доступны по адресам:

| Документ | URL |
|---|---|
| Главная | `https://zcredi.github.io/sleeparchitect-legal/` |
| Privacy Policy (EN) | `https://zcredi.github.io/sleeparchitect-legal/privacy-policy-en.html` |
| Privacy Policy (RU) | `https://zcredi.github.io/sleeparchitect-legal/privacy-policy-ru.html` |
| Terms of Use (EN) | `https://zcredi.github.io/sleeparchitect-legal/terms-of-use-en.html` |
| Terms of Use (RU) | `https://zcredi.github.io/sleeparchitect-legal/terms-of-use-ru.html` |

В App Store Connect → App Privacy → **Privacy Policy URL** → вставь:
`https://zcredi.github.io/sleeparchitect-legal/privacy-policy-en.html`

Для русской локализации (App Information → Localizations → Russian → Privacy Policy URL):
`https://zcredi.github.io/sleeparchitect-legal/privacy-policy-ru.html`

---

## Шаг 4 — Скажи мне когда зальёшь

Я тогда заменю в коде `https://example.com/privacy` и `https://example.com/terms` на реальные ссылки в:
- `SleepArchitect/Views/SettingsView.swift`
- `SleepArchitect/Views/PaywallView.swift`
