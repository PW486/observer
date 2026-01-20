# The Quiet Observer 🏛️

A minimalist sanctuary for deep philosophical thoughts, essays on life, and quiet observations. This project is built with a focus on high-quality content and a seamless, distraction-free reading experience.

[View Live Blog](https://pw486.github.io/observer/)

## ✨ Key Features

- **Philosophical Essays**: A growing collection of profound thoughts on existence, mortality, technology, and the human condition, available in both English and Korean.
- **Dual Language Support**:
  - Automatic language detection based on browser settings.
  - Seamless switching between English and Korean without URL clutter.
  - Persistent language preference via cookies.
- **Enhanced UI/UX**:
  - Minimalist design with a focus on typography and readability.
  - Advanced pagination with grouped navigation and sleek SVG icons.
  - Full mobile optimization for a comfortable reading experience on any device.
  - Dark mode support that respects system preferences and persists across sessions.
- **SEO Optimized**:
  - Dynamic metadata (title and description) updates for every post.
  - Auto-generated `sitemap.xml` and `robots.txt` for search engine visibility.
- **Fast & Lightweight**: Built with Vanilla JavaScript and Markdown for near-instant load times.

## 🚀 Getting Started

### Prerequisites
- Python 3.x (for metadata indexing and local testing)

### Local Development
1. **Clone the repository**:
   ```bash
   git clone https://github.com/PW486/observer.git
   cd observer
   ```
2. **Start a local server**:
   ```bash
   python3 -m http.server 8000
   ```
3. **View the blog**: Open `http://localhost:8000` in your browser.

## ✍️ Writing and Building

### Adding a New Post
1. **Create Markdown files** in the `posts/` directory:
   - `post-id.en.md` (English)
   - `post-id.ko.md` (Korean)
2. **Standard Format**:
   - Title: `# Your Title` (H1)
   - Date: `###### January 20, 2026` (EN) or `###### 2026년 1월 20일` (KO)
3. **Regenerate the index**:
   ```bash
   python3 build.py
   ```
   This script parses the Markdown headers and updates `posts.json` for the frontend.

## 🛠 Project Structure
- `index.html`: Main shell and SEO configuration.
- `style.css`: Design system and responsive styles.
- `script.js`: Routing, state management, and localized content fetching.
- `posts/`: The library of Markdown essays.
- `build.py`: Python tool for automating the metadata index generation.

---
© 2026 The Quiet Observer.