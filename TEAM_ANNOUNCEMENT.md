# 🌍 Time in the Zones - Mindera Office Time Converter

Hey team! 👋

I've built a simple web app to help us coordinate across our global offices. It shows the current time across all Mindera locations and makes it easy to schedule meetings across timezones.

## 🔗 Access the App

**Live URL:** https://mindsimao.github.io/time_in_the_zone/

## ✨ Features

### 1. **Office Locations Display**
View time across all Mindera offices:
- **Portugal** (Porto, Coimbra, Aveiro)
- **United Kingdom** (Leicester, London)
- **Romania** (Cluj-Napoca)
- **India** (Chennai, Bengaluru)
- **Brazil** (Blumenau)
- **United States** (Los Angeles)
- **Morocco** (Casablanca)
- **Vietnam** (Ho Chi Minh)
- **Australia** (Melbourne)

### 2. **Nearest Office Detection**
When you first visit, the app will ask for location permission. If granted, it automatically highlights your nearest Mindera office with a "Nearest Office" badge.

### 3. **Remote Timezone Reference**
Additional cities are grouped by country for remote workers in different timezones (major cities and capitals).

### 4. **Share Specific Times**
Use URL parameters to share specific meeting times with your team:

#### Basic Examples:
- `?time=14:30` - Shows 2:30 PM today (Portugal time by default)
- `?time=09:00&office=India` - Shows 9:00 AM India time across all offices
- `?time=2025-12-25T14:30` - Specific date and time

#### Advanced Examples:
- `?time=15:00&office=Brazil` - What time is it everywhere when it's 3 PM in Brazil?
- `?timezone=America/New_York&time=10:00` - Use a specific timezone as reference
- `?office=Vietnam` - Show current time with Vietnam as reference

## 🎯 Common Use Cases

### Scheduling a Meeting
1. Pick a time in your timezone
2. Add `?time=14:00&office=YourCountry` to the URL
3. Share the link with your team - they'll instantly see what time it is for them

### Quick Time Check
- Just visit the site to see current time across all offices
- Your nearest office is automatically highlighted

### Planning Async Communication
- Check when teams in other offices start/end their day
- Share a URL with a specific time to propose a meeting

## 💡 Tips

- **Bookmark it** - Add to your browser bookmarks for quick access
- **Pin the tab** - Keep it open during your workday
- **Share URLs** - Use query parameters to communicate meeting times clearly
- **No installation needed** - It's just a web page, works everywhere

## 🛠 Technical Details

- Fully client-side (no data collection)
- Works on mobile and desktop
- Updates every second when showing current time
- Respects browser timezone settings
- Uses Intl.DateTimeFormat API for accurate timezone conversion

---

**Questions or suggestions?** Feel free to reach out!

**Made with** ☕ **by Copilot with guidance from Simão**
