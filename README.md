# BioStack Logistics Network Map

An interactive, premium visualization of BioStack's genomic logistics infrastructure across the Mumbai Metropolitan Region (MMR). It maps MOC Cancer Care centers to the central Genomic Analysis Hub.

## Features

- **Leaflet.js Integration**: Fully interactive map utilizing CartoDB Dark Matter tile layer for a high-contrast, premium, dark-mode design.
- **Road-Route Optimization**: The connection lines between MOC centers and the analysis hub follow actual driving road routes fetched dynamically via the OSRM (OpenStreetMap Routing Machine) API.
- **Color-Coded Classification**:
  - 🟡 **Hospital for Patient Recruitment**: Patient recruitment sites where samples are collected and sent to the analysis hub.
  - 🔵 **Sequencing Site**: Advanced centers with potential for setting up sequencing in-house, eliminating logistics time.
  - 🟢 **Analysis Hub**: Located at IIT Bombay (Powai), styled as a distinctive central node.
- **Interactive Details**: Hovering over route lines highlights them and shows precise road transit times + 30-minute sample collection overhead. Clicking a center marker focuses the map and pulls up a detailed information panel with specific workflows.

## Project Structure

```
biostack-map/
└── index.html      # Main application file containing all layout, styling, and JavaScript logic.
```

## Setup & Deployment

Since this project is built entirely in vanilla HTML, CSS, and JS with no build steps or external bundlers, deploying it is trivial:

### Local Preview
Simply open `index.html` in any web browser. (Requires an active internet connection to pull Leaflet libraries and map tiles).

### Deploy to GitHub Pages
1. Create a new repository on your GitHub account.
2. Initialize this directory as a git repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   ```
3. Link to your GitHub remote and push:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git branch -M main
   git push -u origin main
   ```
4. Go to **Settings** > **Pages** in your GitHub repository and select the `main` branch to serve the directory.
