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
- **Work Hours Indicators**: Visual badges showing time status for each location
  - 🟢 **Work Hours** (9 AM - 6 PM weekdays) - Green
  - 🟡 **Early Morning** (6 AM - 9 AM) / **Evening** (6 PM - 10 PM) - Yellow
  - 🟣 **Night** (10 PM - 6 AM) - Purple
  - 🔵 **Weekend** (Saturday/Sunday) - Blue
- **Date & Time Picker**: Built-in UI for selecting custom dates, times, and reference timezones
- **Query Parameters**: Share specific times via URL parameters
- **Live Updates**: Time updates every second when viewing current time
- **Responsive Design**: Works on desktop and mobile devices

## Usage

### Interactive Date & Time Picker

The easiest way to explore different times:

1. **Select a date** using the date picker (optional - defaults to today)
2. **Select a time** using the time picker
3. **Choose an office** from the dropdown to use as reference timezone
4. **Click "Apply"** to update the view
5. **Click "Reset Filters"** to return to current time + Portugal timezone

The URL will automatically update with your selections, making it easy to share.

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
- **Work Hours Indicators**: Color-coded badges for instant status recognition
  - Green for work hours (best time to collaborate)
  - Yellow for early morning/evening (might be available)
  - Purple for night time (avoid contacting unless urgent)
  - Blue for weekends (off days)
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
The work hours indicators will instantly show who's in working hours and who's not.

**OR** use the date/time picker:
1. Select your proposed meeting date and time
2. Choose your office from the dropdown
3. Click "Apply"
4. Check the work hours badges - look for green!
5. Share the URL with invitees

### Quick Time Reference
Keep the page open to quickly check current time across all Mindera offices and see who's available for real-time collaboration.

### Async Communication Planning
- Check when teams in other offices start/end their workday
- See which offices are in "Work Hours" (green badge) for immediate responses
- Identify "Evening" or "Night" zones to plan async communication
- Respect weekend time (blue badge) by scheduling non-urgent messages for Monday

### Before Sending a Message
Quickly glance at the time status:
- **Green (Work Hours)**: Good time to reach out
- **Yellow (Early/Evening)**: They might be available, but check first
- **Purple (Night)**: Send async, expect response later
- **Blue (Weekend)**: Wait until Monday unless urgent

## Privacy

- **No data collection**: Everything runs client-side
- **No tracking**: No analytics or external services
- **Geolocation**: Optional - only used to highlight nearest office, never stored or transmitted

## Contributing

Suggestions and improvements are welcome! This is a simple tool to help Mindera teams coordinate across timezones.

## Credits

© 2025 · Made by Copilot with guidance from Simão
