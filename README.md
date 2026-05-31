# ♛ Jcz Entertainment Platform

Web app streaming premium — Anime Sub Indo + Movie/Series worldwide.
Installable di **Android, iPhone, Laptop** sebagai PWA.

---

## ⬡ Halaman

| File | Keterangan |
|------|-----------|
| `index.html` | Landing page — pilih JczAnime atau JczMovies |
| `anime.html` | JczAnime — streaming anime Sub Indo (Samehadaku via nimeku API) |
| `movie.html` | JczMovies — streaming Movie & TV Series (TMDB + Vidking player) |
| `manifest.json` | PWA config |
| `sw.js` | Service Worker |

---

## ▶ Cara Jalankan

```bash
cd public
python3 -m http.server 8080
# Buka: http://localhost:8080
```

Atau deploy ke Vercel / Netlify / Firebase Hosting (drag & drop folder `public`).

---

## ◈ API yang Digunakan

### JczAnime (anime.html)
- **nimeku API** (`nimeku.vercel.app/api`) — wrapper Samehadaku
  - `/new` — anime terbaru
  - `/popular/page/1` — anime populer
  - `/movie/page/1` — anime movie
  - `/genre/{slug}` — per genre
  - `/search?q=` — search
  - `/anime/detail/{slug}` — detail + episode list
  - `/stream/{episode-slug}` — server streaming

### JczMovies (movie.html)
- **TMDB API** (`api.themoviedb.org/3`) — data film & series
- **Vidking Player** (`vidking.net/embed/movie/{id}`) — player movie
- **Vidking TV** (`vidking.net/embed/tv/{id}/{season}/{ep}`) — player series

---

## 📱 Install sebagai App

### Android → Chrome → ⋮ → Install App
### iPhone  → Safari → Share → Add to Home Screen
### Laptop  → Chrome/Edge → klik ikon install di address bar

---

## ✦ Fitur

**JczAnime:**
- ⬡ Browse anime per genre (Action, Comedy, Fantasy, Romance, dll)
- 🆕 Anime terbaru dari Samehadaku
- 🔍 Search real-time
- ▶ Player multi-server langsung di app
- ⊕ Watchlist personal

**JczMovies:**
- ◉ Movie trending, populer, top rated
- ◈ TV Series dengan pilihan season & episode
- 🔍 Search movie/series
- ▶ Player HD via Vidking (seperti Cineby)
- ⊕ Watchlist personal

---

*♛ Jcz Entertainment — Dark Luxury Streaming Platform*
