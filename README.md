# 🏘️ My Region - Local Events & Places Aggregator

A simple, beautiful web app that aggregates news and events from multiple local websites in the Radotín-Soběchleby area (Olomouc Region, Czech Republic) and surrounding cities up to 100 km.

![Status](https://img.shields.io/badge/status-active-success)
![License](https://img.shields.io/badge/license-MIT-blue)

## ✨ Features

- **📰 Events Tab** - View upcoming events, past events, and announcements from local sources
- **🔗 Sources Tab** - Browse 63+ websites organized by city (loaded from editable JSON)
- **🗺️ Places to Visit Tab** - Checklist of tourist attractions with progress tracking
- **📱 Responsive Design** - Works on desktop, tablet, and mobile
- **🎨 Beautiful UI** - Clean, modern design with smooth animations
- **⚡ No Backend Required** - Pure HTML/CSS/JavaScript, host anywhere

## 🏙️ Cities Covered

| City | Distance | Sources |
|------|----------|---------|
| Radotín | 0 km | 1 |
| Soběchleby, Týn n.B., Teplice n.B., Ústí | 2-8 km | 5 |
| Lipník nad Bečvou | 7 km | 2 |
| Přerov | 14 km | 3 |
| Olomouc | 30 km | 5 |
| Kroměříž | 30 km | 7 |
| Prostějov | 35 km | 6 |
| Zlín | 45 km | 11 |
| Šumperk | 55 km | 7 |
| Ostrava | 70 km | 8 |
| Opava | 85 km | 7 |

## 🚀 Quick Start

1. Download or clone this repository
2. Open `index.html` in your browser
3. That's it! No server needed.

## 📁 Project Structure

```
my-region-app/
├── index.html      # Main app (open this in browser)
├── sources.json    # List of all sources (edit to add/remove)
├── places.json     # Places to visit checklist
└── README.md       # This file
```

## ➕ How to Add a New Source

1. Open `sources.json` in any text editor (Notepad works fine)
2. Add a new entry in the `sources` array:

```json
{
  "city": "Hranice",
  "distance": 10,
  "url": "https://www.mesto-hranice.cz/",
  "type": "web",
  "name": "Město Hranice"
}
```

3. Save the file
4. Refresh the app in your browser

### Source Types

| Type | Icon | Use for |
|------|------|---------|
| `web` | 🌐 | Regular websites |
| `facebook` | f | Facebook pages |
| `instagram` | 📷 | Instagram accounts |
| `linkedin` | in | LinkedIn pages |
| `munipolis` | 📱 | Munipolis app links |

## 🌐 Hosting on GitHub Pages (Free)

1. Fork this repository or create a new one
2. Upload all files (`index.html`, `sources.json`, `places.json`)
3. Go to **Settings** → **Pages**
4. Under "Source", select **main** branch
5. Click **Save**
6. Your app will be live at: `https://yourusername.github.io/my-region/`

## 🛠️ Customization

### Change the Region Name
Edit the header in `index.html`:
```html
<h1>My Region</h1>
<p class="subtitle">Radotín-Soběchleby and surroundings (up to 100 km)</p>
```

### Add New Cities
1. Add sources to `sources.json` with the new city name
2. Optionally add a color in the JavaScript `getCityColor()` function

### Modify Places to Visit
Edit `places.json` to add or remove tourist attractions:
```json
{
  "city": "Olomouc",
  "name": "Holy Trinity Column",
  "category": "UNESCO",
  "description": "35m tall Baroque sculpture"
}
```

## 📸 Screenshots

### Events Tab
Filter events by location and type (Upcoming, Past, Announcements)

### Sources Tab
Browse all 63+ sources organized by city with distance indicators

### Places to Visit Tab
Track your progress visiting local attractions

## 🤝 Contributing

Feel free to:
- Add more sources from the region
- Suggest new features
- Report bugs
- Improve the design

## 📄 License

MIT License - feel free to use, modify, and share!

## 🙏 Acknowledgments

- Sources from official city websites, tourism portals, and social media
- Built with ❤️ for the Olomouc region community

---

**Made for newcomers and locals who want to stay connected with their region** 🇨🇿
