# VAWT Advisor 7.0

**Pre-feasibility tool for Dospel Dragon vertical-axis wind turbines: generation & ROI estimation**
**Інструмент попередньої оцінки генерації та ROI для вертикальних вітрогенераторів Dospel Dragon**

🔗 **[Open the calculator / Відкрити калькулятор](https://vlgook.github.io/vawt-advisor/)**

---

## 🇬🇧 English

### What it is

A standalone web calculator for quick pre-feasibility estimation of VAWT installations based on **Dospel Dragon DTR 1000 / 1000+ / 1500+ / Hybrid** turbines.

Built for partners and clients of **ELKO Ukraine · Project Distribution Department, Energy Solutions Group**.

### Features

- Factory power curves for all four Dragon models (19 RPM→W points, manufacturer-confirmed)
- Rated power at **v = 10 m/s**, controller braking at 11 m/s
- 📍 Mean wind speed **directly from a map** (ERA5 reanalysis 2015–2024, Open-Meteo API)
- Jensen wake model + Frandsen (2006) turbulence correction
- Blockage effect for cross-wind rows + Von Mises wind rose
- 20-year financial model: NPV, DPP, ROI, equipment degradation
- Compare tab: up to 3 configurations side by side with best-value highlighting
- Save & open calculations (JSON with all parameters)
- Fully bilingual UA/EN interface, tooltips and validation (the "Model" theory page is Ukrainian-only)
- Engineering-style design: monospaced figures, technical-documentation look
- Built-in changelog shown after version updates
- Works offline (except the map) — a single HTML file, no dependencies

### Technical details

| Parameter | Value |
|---|---|
| Version | 7.0 |
| Size | 169 KB |
| Dependencies | none (map loads from CDN on demand) |
| Compatibility | Chrome, Firefox, Safari, Edge, iOS Safari, Telegram, Teams |
| Data storage | localStorage / sessionStorage (device-local) |

### Physical models

- **Jensen (1983)** — wake with linear cone expansion
- **Frandsen (2006)** — turbulence effect: `kw_eff = kw + 0.5 × TI`
- **Von Mises** — statistical wind rose with concentration parameter κ
- **Weibull** — wind speed distribution for annual generation
- **Dabiri (Caltech, 2011)** — blockage effect for VAWT farms
- **ERA5 reanalysis** — wind climatology (Open-Meteo API, 2015–2024)

Accuracy: ±20–30% (pre-feasibility). Project decisions require an on-site wind survey.

---

## 🇺🇦 Українська

### Що це

Автономний веб-калькулятор для швидкої попередньої оцінки інсталяцій VAWT на базі турбін **Dospel Dragon DTR 1000 / 1000+ / 1500+ / Hybrid**.

Розроблено для партнерів і клієнтів **ELKO Ukraine · Департамент проєктної дистрибуції, група енергетичних рішень**.

### Можливості

- Паспортні криві потужності всіх чотирьох моделей Dragon (19 точок RPM→W, підтверджено виробником)
- Номінальна потужність при **v = 10 м/с**, гальмування контролера при 11 м/с
- 📍 Визначення середньої швидкості вітру **прямо з карти** (ERA5 reanalysis 2015–2024, Open-Meteo API)
- Модель вітрової «тіні» Jensen + поправка на турбулентність Frandsen (2006)
- Ефект підпору при поперечному вітрі + роза вітрів Von Mises
- 20-річна фінансова модель: NPV, DPP, ROI, зношування обладнання
- Вкладка «Порівняти»: до 3 конфігурацій поруч з підсвічуванням найкращих значень
- Збереження та відкриття розрахунків (JSON з усіма параметрами)
- Повна двомовність UA/EN: інтерфейс, тултіпи, валідація (сторінка «Модель» — українською)
- Інженерний дизайн: моноширинні цифри, стиль технічної документації
- Журнал змін: при оновленні версії користувач бачить що саме змінилось
- Працює офлайн (крім карти) — один HTML-файл без залежностей

### Історія версій / Version history

| Версія | Ключові зміни / Key changes |
|---|---|
| **7.0** | Повна двомовність UA/EN, вкладка «Порівняти», збереження розрахунку (JSON), блокування паспортних полів, інженерний редизайн, журнал змін, посилений захист вводу |
| 6.0 | Карта ERA5, v_nominal=10 м/с (уточнення виробника), гальмування при 11 м/с, iOS/Telegram/Teams fixes |
| 5.x | Сторінка «Модель», Frandsen TI, κ=5 дефолт, мініфікація |
| 4.x | Крос-валідація полів, нові попередження |
| 3.x | Jensen wake, Von Mises, blockage, 4 пресети Dragon |

---

## Contact / Контакт

📧 [energy@elko.ua](mailto:energy@elko.ua)

**Volodymyr Huk / Володимир Гук** · BDM · ELKO Ukraine · Project Distribution Department

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Volodymyr%20Huk-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/vladimirguk/)

---

*VAWT Advisor is a pre-feasibility estimation tool. Results are indicative.*
*VAWT Advisor є інструментом попередньої оцінки. Результати носять довідковий характер.*
