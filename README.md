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

## Technical Details

- Pure HTML/CSS/JavaScript (no dependencies)
- Uses Reddit's public JSON API
- Stores preferences in localStorage
- Responsive design with CSS variables
- Supports iOS safe areas and PWA features

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
