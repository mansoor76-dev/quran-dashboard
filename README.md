# 📖 Quran Thematic Dashboard

An interactive, self-contained web dashboard that organizes the major categories, themes, and subjects of the Holy Quran — with a searchable surah index, the 99 Names of Allah, curated ayah references per theme, **live translations**, and **audio recitation**.

**🔗 Live demo:** _enable GitHub Pages to get your link (see below)_

![Made with HTML/CSS/JS](https://img.shields.io/badge/Made%20with-HTML%20%2F%20CSS%20%2F%20JS-38bdf8)
![No build step](https://img.shields.io/badge/Build-None%20(single%20file)-2dd4bf)

---

## ✨ Features

- **🗂️ Themes view** — 32 topic cards across 9 categories (Core Beliefs, Prophets, Worship, Values & Ethics, Law & Society, Signs in Creation, Stories & Parables, Key Surahs) with live search + category filters.
- **📿 Associated ayahs** — each theme expands to show 7–8 curated verse references with short descriptions.
- **🌐 Live translations** — pulls Arabic (Uthmani) + English from the [quran.com API](https://api-docs.quran.com/), with a **translation selector** (Saheeh International, The Clear Quran, Yusuf Ali, Pickthall).
- **🎙️ Audio recitation** — per-verse playback with a **reciter dropdown** (Alafasy, Sudais, Shuraim, Husary, Shatri).
- **🎵 Mini player bar** — floating transport controls (prev / play-pause / next), current-verse label, and repeat counter.
- **🔁 Repeat mode** — repeat each verse ×1–×10 for memorization (hifz).
- **▶ Play all** — recite an entire category in sequence.
- **📜 Surah Index** — all 114 surahs (name, meaning, Meccan/Medinan, ayah count) with search + direct quran.com links.
- **🕌 99 Names of Allah** — full Asma-ul-Husna grid with Arabic, transliteration, and meaning.
- **⬇️ Offline mode** — preload translations + audio (cached via `localStorage` + Cache API) so it works without internet.
- **🖨️ Print / PDF** — clean print stylesheet for a paper-friendly reference.

---

## 🚀 Run it

It's a **single HTML file** — no build, no dependencies.

```bash
# just open it
open index.html      # macOS
# or double-click index.html in your file browser
```

> Live translation/audio need an internet connection on first use; after **⬇️ Preload offline**, cached content works offline.

---

## 🌍 Publish with GitHub Pages

1. Push this repo to GitHub (see below).
2. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
3. Branch: **main** · Folder: **/ (root)** → **Save**.
4. Your dashboard goes live at `https://<your-username>.github.io/<repo-name>/`.

---

## 📚 Data sources & accuracy

- **Text & audio:** [quran.com API v4](https://api-docs.quran.com/) — authentic, fetched live (not transcribed).
- **Surah metadata:** standard Hafs numbering.
- **99 Names:** the popular al-Tirmidhi enumeration (scholars' traditional lists vary slightly).
- Ayah **references + descriptions** are an educational index; always confirm exact text at [quran.com](https://quran.com).

> ⚠️ This dashboard is an educational overview, **not** a source for religious rulings. For anything you rely on, verify against an authenticated Mushaf or a qualified scholar.

---

## 🛠️ Tech

Vanilla **HTML + CSS + JavaScript**. No frameworks, no build tooling. All state cached client-side (`localStorage` + Cache API). Nothing is sent to any server except read-only calls to the public quran.com API.

---

## 📄 License

Released under the [MIT License](LICENSE). The Quran text and audio are the property of their respective sources (quran.com and reciters); this project only links to / fetches them.

---

## 🤝 Contributing

Issues and PRs welcome — especially additional curated ayah references, more translations/reciters, or accessibility improvements.
