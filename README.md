# 📸 Instagram Clone — Pure HTML & CSS

> Trust the process. The result speaks for itself.

Instagram clone built from scratch with pure HTML & CSS — including the left sidebar, middle feed, and right column all hand-structured. Features like-post, save-post, search panel, and notifications panel powered by AI. Zero external CSS libraries used.

## 📁 Project Structure

```
instagram-clone/
├── index.html       # Full app markup with semantic structure & comments
└── index.css        # All styles — layout, components, animations & responsiveness
```


## ✨ Features

### 🏗️ Built Entirely From Scratch
- **Left Sidebar** — navigation with active states, icon switching, logo, and profile section
- **Middle Feed** — stories bar with circular avatars, post cards with actions
- **Right Column** — suggested profiles and account info
- **Mobile Bottom Nav** — responsive navigation bar for smaller screens

### 🤖 AI-Powered Features
- **Like a Post** — heart interaction powered by AI
- **Save a Post** — bookmark interaction powered by AI

### 🎛️ Pure CSS Panel System
- **Search Panel** — slides in as a smooth drawer from the sidebar with a styled search input
- **Notifications Panel** — fully functional notification feed, toggled with zero JavaScript
- Both panels use hidden `<input type="radio">` + the CSS **general sibling selector (`~`)** — no JS at all

### 📱 Fully Responsive
- Sidebar collapses on smaller screens
- Mobile nav bar appears at the bottom
- Feed and layout reflow across all screen sizes

---

## 🧠 How the CSS Panel Trick Works

One of the coolest parts of this project — the Search and Notifications panels open and close without a single line of JavaScript.

```html
<!-- Hidden radio inputs act as state -->
<input type="radio" name="app-panel" id="panel-search" class="state-input">

<!-- CSS listens to :checked state -->
```
```css
#panel-search:checked ~ .app-layout .search-drawer {
  transform: translateX(0); /* slides in */
}
```

The sidebar labels act as the toggle buttons — clicking them checks the radio input, and CSS does the rest.

---

## 🎨 CSS Highlights

This project was as much a **learning journey** as it was a build. New CSS properties were discovered, understood, and applied in real time. Some notable techniques used:

| Technique | Where Used |
|---|---|
| CSS Custom Properties (`:root` variables) | Theming — colors, widths, font stack |
| `cubic-bezier` easing | Smooth drawer & sidebar transitions |
| SVG data URI in `background-image` | Search input icon without an extra element |
| General sibling selector (`~`) | Panel toggle system without JavaScript |
| Flexbox | Almost every layout component |
| `position: fixed` + `transform` | Sliding drawers and sidebar |
| `:checked` pseudo-class | Active nav states and panel switching |
| `transition` + `transform` | Hover effects, icon scaling, panel animations |
| `object-fit: cover` | Consistent avatar and post image rendering |
| `overflow: hidden` + `border-radius` | Circular avatars and rounded cards |

---

## 💬 Code Readability

Every section across both `index.html` and `index.css` is **thoroughly commented** — making it easy to navigate, understand the intent behind each block, and build on top of it.

```css
/* Sidebar */
.sidebar { ... }

/* Drawers */
.search-drawer,
.notifications-drawer { ... }

/* Feed */
.feed-post { ... }
```

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Semantic structure, accessibility attributes |
| CSS3 | All layout, styling, animations, responsiveness |
| AI | Like & save post features |

> ⚠️ The only JavaScript present is a tiny scroll-button visibility handler for the stories strip. Everything else is pure CSS.

---

## 📸 Screenshots
<img width="1917" height="907" alt="image" src="https://github.com/user-attachments/assets/8ee21648-06c2-405e-a4a9-3a361e873d5b" />
<img width="1917" height="902" alt="image" src="https://github.com/user-attachments/assets/f111faec-4b5d-45d1-bf95-a8a78886d9d4" />
<img width="1917" height="905" alt="image" src="https://github.com/user-attachments/assets/c714576f-27e3-4c3b-9d12-2e397c01d93f" />
<img width="1917" height="906" alt="image" src="https://github.com/user-attachments/assets/246121e6-a9ba-4a61-99e8-07989e638381" />
<img width="1917" height="902" alt="image" src="https://github.com/user-attachments/assets/9d09a776-8de3-4e25-a3e2-f642bb39f16a" />
<img width="1917" height="897" alt="image" src="https://github.com/user-attachments/assets/fcd74f66-9d43-4928-8193-90cb3d9f17d4" />





## 🙌 Author

Made with curiosity and a lot of CSS by Harshit Singh
