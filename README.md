# Reddit Reader

A lightweight, mobile-friendly web app that replicates the Reddit "Home" feed experience without requiring login. Perfect for iPhone users who want to browse their favorite subreddits.

## Features

- **No login required** - Browse Reddit without an account
- **Custom subreddit list** - Add/remove your favorite subreddits (saved in localStorage)
- **Combined feed** - View posts from all your subreddits in one feed
- **Filter by subreddit** - Tap tabs to view posts from a specific subreddit
- **Mobile-optimized** - Designed specifically for iPhone with:
  - Safe area support for notched devices
  - Touch-friendly interface
  - Pull-to-refresh
  - Infinite scroll
  - Add to Home Screen support
- **Media support** - Images, videos, and link previews
- **Reddit-like UI** - Familiar card-based layout with upvotes and comments

## Usage

1. Open `index.html` in your iPhone's Safari browser
2. Add to Home Screen for an app-like experience:
   - Tap the Share button
   - Select "Add to Home Screen"
3. Tap the gear icon to manage your subreddits
4. Pull down to refresh the feed
5. Tap a subreddit tab to filter posts

## Default Subreddits

The app comes pre-configured with these subreddits:
- r/funny
- r/pics
- r/news
- r/technology
- r/askreddit

You can add or remove any subreddit through the settings modal.

## Installing as an App on iPhone

This is a Progressive Web App (PWA) that can be installed on your iPhone:

1. **Generate icons first** (one-time setup):
   - Open `generate-icons.html` in any browser
   - Click "Download All Icons"
   - Save the files to the `icons/` folder

2. **Deploy to GitHub Pages** (see Hosting section below)

3. **Install on iPhone**:
   - Open Safari and navigate to your GitHub Pages URL
   - Tap the **Share** button (square with arrow)
   - Scroll down and tap **Add to Home Screen**
   - Name it "Reddit Reader" and tap **Add**

The app will now appear on your home screen with its own icon and launch in full-screen mode like a native app.

## Technical Details

- Pure HTML/CSS/JavaScript (no dependencies)
- Progressive Web App (PWA) with offline support
- Uses Reddit's public JSON API
- Stores preferences in localStorage
- Responsive design with CSS variables
- Supports iOS safe areas and standalone mode

## Hosting

To use on your iPhone, you can:

1. **Local server** - Run a local HTTP server and access via your local network
2. **GitHub Pages** - Push to GitHub and enable Pages
3. **Any static host** - Deploy to Netlify, Vercel, or any static file host

Example with Python:
```bash
python3 -m http.server 8000
```

Then open `http://your-ip:8000` on your iPhone.

## License

MIT
