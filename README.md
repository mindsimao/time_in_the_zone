# Time in the Zone

A timezone converter application that displays time across multiple Mindera office locations and remote timezones worldwide.

## Features

- **Reference Time**: Portugal (Porto, Coimbra, Aveiro, Lisboa)
- **Office Locations**: Leicester, London, Cluj-Napoca, Chennai, Bengaluru, Blumenau, Los Angeles, Casablanca, Ho Chi Minh, Melbourne
- **Remote Timezones**: Additional cities grouped by country for remote workers
- **Query Parameters**: Pass specific time via URL parameters

## Usage

### View Current Time
Simply open the page:
```
https://simaob.github.io/time_in_the_zone/
```

### View Specific Time
Pass time as a query parameter:
```
https://simaob.github.io/time_in_the_zone/?time=14:30
```

### View Specific Date & Time
Pass full ISO 8601 format:
```
https://simaob.github.io/time_in_the_zone/?time=2025-01-15T14:30
```

## GitHub Pages Setup

To enable GitHub Pages for this repository:

1. Go to your repository on GitHub: `https://github.com/simaob/time_in_the_zone`
2. Click on **Settings**
3. Scroll down to **Pages** section in the left sidebar
4. Under **Source**, select **Deploy from a branch**
5. Select branch **main** and folder **/ (root)**
6. Click **Save**
7. Wait a few minutes for the deployment to complete
8. Your site will be available at: `https://simaob.github.io/time_in_the_zone/`

## Design

The application features a dark theme with gold accents inspired by Mindera's brand identity, providing a clean and professional interface for viewing times across global locations.

## Technologies

- Pure HTML5
- CSS3 with modern features (Grid, Flexbox, CSS Variables)
- Vanilla JavaScript (no dependencies)
- Intl.DateTimeFormat API for timezone handling
