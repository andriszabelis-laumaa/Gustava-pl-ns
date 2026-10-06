# ⚔️ Quest Log — misiju plānotājs

Spēles stila ikdienas uzdevumu plānotājs: misijas, XP, līmeņi, 🔥 sērijas, trofejas un monētu veikals ar balvām. Misijas apstiprina vecāki.

## Misijas

| Misija | Dienas | XP |
|---|---|---|
| 👕 Pārģērbties pēc skolas | P–Pk | 10 |
| 🍽️ Izkrāmēt traukus | katru dienu | 15 |
| 📚 Mācības, mājas darbi (1–2 h) | katru dienu (📖 sestdiena — mācīšanās diena) | 30 |
| ⚽ Sports | T 17:00–18:30, C 16:30–18:00, Pk 15:00–16:30 | 30 |
| 🧹 Sakārtot istabu, drēbes skapī | katru dienu | 20 |
| 🧩 Uzdevumi.lv *(bonuss)* | katru dienu | 10 |
| 🤝 Laiks ar draugiem *(brīvprātīgi)* | katru dienu | — |
| 🎮 Brīvais laiks *(atbloķējas pēc obligātajām)* | katru dienu | 5 |

**Ideāla diena** (visas obligātās misijas apstiprinātas) = +70 XP bonuss un 🔥 sērija turpinās.

**🤫 Klusais laiks 21:00–22:00** — ja netiek ievērots, vecāki ieķeksē ailē "Netika": −20 XP.

**⚠️ Nepieņemama uzvedība** — vecāki var dot sodu −20 XP.

## Kā tas strādā

- Katrai misijai ir divas ailes: **🧒 Es** un **👨‍👩‍👦 Vecāki**.
- **Bērns** ieķeksē savu aili → misija ⏳ *gaida apstiprinājumu*. XP tiek piešķirts tikai, kad vecāki ieķeksē savu aili.
- Bērns var atzīmēt tikai **šodienas** misijas. Iepriekšējās dienas var labot tikai vecāki.
- **Vecāki**, pirmo reizi spiežot vecāku aili, ievada PIN (pirmajā reizē to iestata). Tad 10 min var ķeksēt brīvi:
  - apstiprināt misijas un ieķeksēt klusā laika pārkāpumu;
  - apstiprināt iepriekšējo dienu misijas un dot sodu par uzvedību;
  - 📅 Mēneša tabulā labot jebkuru pagājušo dienu;
  - importēt datus un sākt no jauna.
- Vecāku režīms aizveras pats pēc 10 min.

> Svarīgi: apstiprināšana notiek **tajā pašā ierīcē**, kur bērns lieto lietotni (dati glabājas pārlūkā).

## Veikals

| Balva | Cena |
|---|---|
| 🎮 +30 min spēļu laika | 400 🪙 |
| 🍫 Mīļākais našķis | 250 🪙 |
| 🌙 +30 min vēlāk gulēt (brīvdienās) | 400 🪙 |
| 🎬 Filmu vakars — tu izvēlies filmu | 800 🪙 |
| 🏆 Lielā balva (vienojies ar vecākiem) | 3500 🪙 |

## Publicēšana GitHub Pages

1. Augšupielādē `index.html` un `README.md` repozitorijā.
2. **Settings → Pages → Source: Deploy from a branch**, branch `main`, mape `/ (root)` → Save.
3. Pēc ~1 min lapa būs pieejama `https://<lietotājs>.github.io/<repozitorijs>/`.
4. Telefonā atver saiti un izvēlies **"Pievienot sākuma ekrānam"**.

## Pielāgošana

Viss maināms faila `index.html` sākumā, sadaļā `KONFIGURĀCIJA`:

- `TASKS` — misijas, ikonas, XP un dienas (`0` = svētdiena … `6` = sestdiena); `approve:false` — bez vecāku apstiprinājuma
- `PERFECT_BONUS`, `PENALTY_REASONS`, `QUIET`, `LEARN_DAY` — bonuss, sodi, klusais laiks, mācīšanās diena
- `REWARDS` — veikala balvas un cenas

## Dati

Progress glabājas pārlūkā (localStorage). Sadaļā ⚙️ **Iestatījumi** var eksportēt rezerves kopiju (JSON); importēt un dzēst var tikai vecāku režīmā.
