# Admin Dashboard

A responsive admin dashboard UI built with plain HTML and CSS Grid, based on The Odin Project's "Admin Dashboard" project. Recreates a common real-world layout pattern: fixed sidebar, header, and a main content area with a projects grid and a secondary sidebar.

## Live Demo

_Add your GitHub Pages link here once deployed._

## Preview

_Add a screenshot here, e.g. `![Dashboard preview](images/preview.png)`_

## Features

- **Sidebar navigation** with icon + label menu items, split into primary links (Home, Profile, Messages, History, Tasks, Communities) and secondary links (Settings, Support, Privacy)
- **Header** with a search bar, notification icon, and user profile
- **Welcome banner** with quick-action buttons (New, Upload, Share)
- **Projects grid** of responsive cards, each with a title, description, and action icons (favorite, view, share)
- **Announcements panel** listing recent updates
- **Trending panel** showing popular users/projects
- Fully responsive grid layout using CSS Grid (no media queries needed at this stage)

## Tech Stack

- HTML5
- CSS3 (Grid & Flexbox)
- [Google Material Icons](https://fonts.google.com/icons)

## Project Structure

```
├── index.html
├── style.css
└── images/
    ├── profile.png
    ├── user1.png
    ├── user2.png
    └── user3.png
```

## Layout Approach

- The overall page uses a **2-column CSS Grid** (`1fr 4fr`) to split the sidebar from the main content.
- The main section uses a **2-row grid** (`2fr 8fr`) to separate the header from the content area.
- The content area uses another **grid** (`3fr 1fr`) to place the projects section next to the right sidebar.
- The projects grid uses `repeat(auto-fill, minmax(200px, 1fr))` so cards automatically wrap and resize based on available space.

## What I Practiced

- Nesting multiple CSS Grid containers within each other
- Building consistent, reusable card components
- Structuring semantic HTML (`aside`, `nav`, `main`, `header`, `section`, `article`)
- Using Material Icons alongside text for a cleaner UI

## Known Issues / To Do

- [ ] Add real profile/user images (currently placeholder paths in `images/`)
- [ ] Add responsive breakpoints for smaller screens (currently optimized for desktop)
- [ ] Make sidebar and button elements interactive (currently static markup)

## Acknowledgements

Project brief from [The Odin Project](https://www.theodinproject.com/) — Full Stack JavaScript path, HTML & CSS course.
