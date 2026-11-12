# Pokretanje InFON Frontenda

## Preduslovi

- **Node.js** (v18+) – preuzmite sa [nodejs.org](https://nodejs.org)
- **npm** (dolazi uz Node.js)

## Instalacija i pokretanje

```bash
# Uđite u frontend direktorijum
cd C:\Users\DS003\Desktop\InFON\frontend

# Instalirajte zavisnosti
npm install

# Pokrenite razvojni server
npm run dev
```

Aplikacija će biti dostupna na: **http://localhost:5173**

## Demo pristup

| Rola | Email | Lozinka |
|------|-------|---------|
| Admin | admin@fon.bg.ac.rs | admin123 |
| Profesor | profesor@fon.bg.ac.rs | prof123 |

## Struktura projekta

```
frontend/
├── src/
│   ├── App.jsx              # Routing
│   ├── main.jsx             # Entry point
│   ├── index.css            # Global styles + Tailwind
│   ├── components/
│   │   ├── Navbar.jsx       # Navigacija sa hamburger menijem
│   │   ├── EventCard.jsx    # Kartica događaja sa modalnim prozorom
│   │   ├── EventList.jsx    # Grid kartica
│   │   ├── EventCalendar.jsx# FullCalendar prikaz
│   │   ├── FilterBar.jsx    # Filteri po organizatoru/tipu/datumu
│   │   ├── OrganizerBadge.jsx # Badge organizatora
│   │   └── ExportButton.jsx # PDF/CSV export
│   ├── pages/
│   │   ├── Home.jsx         # Glavna stranica
│   │   ├── Login.jsx        # Forma za prijavu
│   │   └── AdminDashboard.jsx # Admin panel
│   ├── context/
│   │   └── AuthContext.jsx  # Autentifikacija (localStorage)
│   └── data/
│       └── mockData.js      # 16 mock događaja, 7 organizatora
```
