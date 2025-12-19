# Time in the Zone

A timezone converter application that displays time across multiple Mindera office locations and remote timezones worldwide.

## 🔗 Live Demo

**https://mindsimao.github.io/time_in_the_zone/**

## Features

- **Reference Time**: Portugal (Porto, Coimbra, Aveiro, Lisboa) - default reference timezone
- **Office Locations**: All Mindera offices grouped by country
  - Portugal: Porto, Coimbra, Aveiro
  - United Kingdom: Leicester, London
  - Romania: Cluj-Napoca
  - India: Chennai (Kotturpuram & Thiruvanmiyur), Bengaluru
  - Brazil: Blumenau
  - United States: Los Angeles
  - Morocco: Casablanca
  - Vietnam: Ho Chi Minh
  - Australia: Melbourne
- **Remote Timezones**: Additional cities grouped by country for remote workers
- **Geolocation**: Automatically highlights your nearest Mindera office
- **Query Parameters**: Share specific times via URL parameters
- **Live Updates**: Time updates every second when viewing current time
- **Responsive Design**: Works on desktop and mobile devices

## Usage

### View Current Time
Simply open the page:
```
https://mindsimao.github.io/time_in_the_zone/
```

### View Specific Time
Pass time as a query parameter:
```
https://mindsimao.github.io/time_in_the_zone/?time=14:30
```

### View Specific Date & Time
Pass full ISO 8601 format:
```
https://mindsimao.github.io/time_in_the_zone/?time=2025-01-15T14:30
```

### Use Different Reference Timezone
Use the `office` parameter to set a different office as reference:
```
https://mindsimao.github.io/time_in_the_zone/?time=09:00&office=India
```

This shows what time it is everywhere when it's 9:00 AM in India.

### Advanced Examples

- `?office=Brazil` - Show current time with Brazil as reference
- `?time=15:00&office=Vietnam` - Show 3 PM Vietnam time across all offices
- `?timezone=America/New_York&time=10:00` - Use custom timezone as reference
- `?time=2025-12-25T14:30&office=Morocco` - Specific date/time in Morocco timezone

## Query Parameters

| Parameter | Alias | Description | Example |
|-----------|-------|-------------|---------|
| `time` | - | Specific time to display | `?time=14:30` |
| `timezone` | `tz` | Custom timezone for reference | `?timezone=America/New_York` |
| `office` | - | Use office location as reference | `?office=India` |

## GitHub Pages Setup

To enable GitHub Pages for this repository:

1. Go to your repository on GitHub
2. Click on **Settings**
3. Scroll down to **Pages** section in the left sidebar
4. Under **Source**, select **Deploy from a branch**
5. Select branch **main** and folder **/ (root)**
6. Click **Save**
7. Wait a few minutes for the deployment to complete
8. Your site will be available at the configured GitHub Pages URL

## Design

The application features a dark theme with gold accents inspired by Mindera's brand identity, providing a clean and professional interface for viewing times across global locations.

### Key Design Elements

- **Office Locations**: Highlighted with gold borders and enhanced styling
- **Remote Timezones**: Grouped by country for cleaner organization
- **Nearest Office**: Automatically detected via geolocation with special badge
- **Hover Effects**: Smooth transitions and visual feedback
- **Responsive Grid**: Adapts to different screen sizes

## Technologies

- **HTML5**: Semantic markup
- **CSS3**: Modern features (Grid, Flexbox, CSS Variables, Gradients)
- **Vanilla JavaScript**: No dependencies
- **Intl.DateTimeFormat API**: Native timezone handling
- **Geolocation API**: Nearest office detection

## Use Cases

### Scheduling Meetings
Share a URL with your proposed meeting time to help teammates see it in their timezone:
```
?time=14:00&office=Portugal
```

### Quick Time Reference
Keep the page open to quickly check current time across all Mindera offices.

### Async Communication Planning
Check when teams in other offices start/end their workday to optimize communication timing.

## Privacy

- **No data collection**: Everything runs client-side
- **No tracking**: No analytics or external services
- **Geolocation**: Optional - only used to highlight nearest office, never stored or transmitted

## Contributing

Suggestions and improvements are welcome! This is a simple tool to help Mindera teams coordinate across timezones.

## Credits

© 2025 · Made by Copilot with guidance from Simão
