# LevelUp Gaming Community

Course project (IT Web Design). A multi-page gaming community site with
tournament listings, a stream team showcase, member registration, and
a contact form.

Live demo: https://alexstaplesdesign.github.io/levelup-gaming-community/

## Stack

HTML5 · CSS3 · JavaScript (vanilla) · Font Awesome · Google Fonts

## Pages

| File | Description |
|------|-------------|
| `index.html` | Homepage — featured games, tournament preview, community stats |
| `about.html` | Team profiles and mission |
| `games.html` | Games showcase |
| `events.html` | Upcoming tournaments |
| `community.html` | Stream team and member spotlights |
| `contact.html` | Contact form |
| `register.html` | Registration (two versions: hero and mobile) |
| `secretpageunlocked.html` | Easter egg — find it yourself |

## Running it

No build step — open `index.html` in a browser, or:

```bash
python -m http.server 8000
```

## CSS structure

Modular — one file per page plus shared base files:

```
css/
├── base.css        # Variables, reset, utilities
├── navigation.css
├── footer.css
├── home.css
├── about.css
├── games.css
├── events.css
├── community.css
├── contact.css
└── register.css
```

CSS custom properties handle the color system:

```css
--primary-color: #4169e1;
--secondary-color: #8a2be2;
--accent-color: #ff7f50;
```

## JavaScript (`js/script.js`)

- Mobile hamburger nav with body scroll lock while menu is open
- Closes nav on link click or outside click
- Smooth anchor scrolling
- Form validation with real-time error highlighting — required fields,
  email format, password confirmation match
- On valid submit: 1.5s loading state, then the form fades out and
  is replaced with a thank-you message (no page reload)
- Error popup for invalid submissions (auto-dismisses after 5s)
- Card hover lift effect
- AOS animation support if the library is loaded
