# 🐿️ Squirrel Sweep

A fun, forest-themed minesweeper game where you find acorns and avoid squirrels!

## Features

- 🎮 Three difficulty levels (Easy, Medium, Hard)
- ⏱️ Built-in timer
- 🌰 Flag system for marking suspected squirrels
- 📱 Fully responsive design
- 🎨 Beautiful woodland aesthetic
- ⚡ No dependencies - pure vanilla HTML/CSS/JavaScript

## Game Rules

1. **Left-click** to reveal a cell
2. **Right-click** to place/remove a flag
3. Numbers indicate how many squirrels are adjacent to that cell
4. Reveal all safe cells to win
5. Find a squirrel and it's game over!

## Difficulty Levels

| Level  | Size   | Squirrels |
|--------|--------|-----------|
| Easy   | 8×8    | 10        |
| Medium | 12×12  | 30        |
| Hard   | 16×16  | 40        |

## Deployment to GitHub Pages

### Method 1: Using GitHub Pages (Recommended)

1. **Create a new repository** on GitHub called `squirrel-sweep` (or any name)

2. **Clone the repository** to your computer:
   ```bash
   git clone https://github.com/YOUR-USERNAME/squirrel-sweep.git
   cd squirrel-sweep
   ```

3. **Add the files**:
   ```bash
   # Copy the index.html file to your repository
   cp index.html .
   git add index.html
   git commit -m "Add Squirrel Sweep game"
   git push origin main
   ```

4. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click **Settings** → **Pages**
   - Under "Build and deployment", select **Deploy from a branch**
   - Choose **main** branch and **/ (root)** folder
   - Click **Save**

5. **Wait a minute** for deployment to complete, then visit:
   ```
   https://YOUR-USERNAME.github.io/squirrel-sweep/
   ```

### Method 2: Deploy to a Custom Domain

1. Follow steps 1-3 above
2. In the GitHub Pages settings, add your custom domain
3. Update your domain's DNS settings to point to GitHub Pages (see [GitHub docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site))

### Method 3: Deploy to Other Hosting Services

Since this is a single HTML file, you can also deploy to:

- **Netlify**: Drag and drop `index.html` to https://app.netlify.com
- **Vercel**: Upload the file to https://vercel.com
- **Firebase Hosting**: Follow [Firebase deployment guide](https://firebase.google.com/docs/hosting)
- **Any static hosting service**

## Local Development

Simply open `index.html` in your web browser:

```bash
# On macOS
open index.html

# On Windows
start index.html

# On Linux
xdg-open index.html
```

Or use a local server:

```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (with http-server installed)
npx http-server
```

Then visit `http://localhost:8000`

## Customization

You can easily customize the game by editing the CSS and JavaScript in `index.html`:

### Change Colors
Look for the color variables in the `<style>` section:
- `#2d5016` - Primary green color
- `#4a7c2c` - Background gradient color
- `#d32f2f` - Red warning color
- `#fff3cd` - Yellow flag color

### Adjust Difficulty Settings
Modify the `settings` object in the `<script>` section:
```javascript
const settings = {
    easy: { size: 8, squirrels: 10 },
    medium: { size: 12, squirrels: 30 },
    hard: { size: 16, squirrels: 40 }
};
```

### Change Cell Size
Update the `.cell` width and height in the CSS (default is 40px)

## Browser Support

Works on all modern browsers:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## License

Free to use and modify for personal or commercial projects.

## Credits

Made with 🌰 by Squirrel Sweep

## Contributing

Found a bug or have an idea? Feel free to:
1. Fork the repository
2. Create a new branch for your feature
3. Make your changes
4. Submit a pull request

## Questions?

Open an issue on the GitHub repository and I'll help!

---

Enjoy the game! 🐿️🌰