# ⚔️ Quest Log — misiju plānotājs

Spēles stila ikdienas uzdevumu plānotājs: misijas, XP, līmeņi, 🔥 sērijas, trofejas un monētu veikals ar balvām.

## Misijas

| Misija | Dienas | XP |
|---|---|---|
| 👕 Pārģērbties pēc skolas | P–Pk | 10 |
| 🍽️ Izkrāmēt traukus | katru dienu | 15 |
| 📚 Mācības, mājas darbi | Sv–Pk | 30 |
| ⚽ Sports | T 17:00–18:30, C 16:30–18:00, Pk 15:00–16:30 | 30 |
| 🧹 Sakārtot istabu, drēbes skapī | katru dienu | 20 |
| 🧩 Uzdevumi.lv *(bonuss)* | katru dienu | 10 |
| 🤝 Laiks ar draugiem *(brīvprātīgi)* | katru dienu | — |
| 🎮 Brīvais laiks *(atbloķējas pēc obligātajām)* | katru dienu | 5 |

**Ideāla diena** (visas obligātās misijas izpildītas) = +70 XP bonuss un 🔥 sērija turpinās.

## Publicēšana GitHub Pages

1. Izveido jaunu repozitoriju, piem. `quest-log`.
2. Augšupielādē `index.html` (un šo `README.md`).
3. **Settings → Pages → Source: Deploy from a branch**, branch `main`, mape `/ (root)` → Save.
4. Pēc ~1 min lapa būs pieejama: `https://<lietotājs>.github.io/quest-log/`
5. Telefonā atver saiti un izvēlies **"Pievienot sākuma ekrānam"** — tad tā strādā kā lietotne.

## Pielāgošana

Viss maināms faila `index.html` sākumā, sadaļā `KONFIGURĀCIJA`:

- `TASKS` — misijas, ikonas, XP un dienas (`0` = svētdiena … `6` = sestdiena)
- `PERFECT_BONUS` — ideālās dienas bonuss
- `REWARDS` — veikala balvas un to cenas monētās

## Dati

Progress glabājas pārlūkā (localStorage) tajā ierīcē, kur lapa atvērta. Sadaļā ⚙️ **Iestatījumi** var eksportēt/importēt rezerves kopiju (JSON), piem., pārejot uz citu telefonu.
