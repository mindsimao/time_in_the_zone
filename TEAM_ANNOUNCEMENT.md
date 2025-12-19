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

### 2. **Work Hours Indicators**
Each location shows a color-coded badge indicating the time status:
- 🟢 **Work Hours** (9 AM - 6 PM weekdays) - Best time to collaborate
- 🟡 **Early Morning/Evening** (6-9 AM or 6-10 PM) - Might be available
- 🟣 **Night** (10 PM - 6 AM) - Avoid unless urgent
- 🔵 **Weekend** (Saturday/Sunday) - Off days

### 3. **Date & Time Picker**
Use the built-in picker to:
- Select a specific date and time
- Choose a reference office/timezone
- See what time it will be everywhere at that moment
- Click "Reset Filters" to return to current time

### 4. **Nearest Office Detection**
When you first visit, the app will ask for location permission. If granted, it automatically highlights your nearest Mindera office with a "Nearest Office" badge.

### 5. **Remote Timezone Reference**
Additional cities are grouped by country for remote workers in different timezones (major cities and capitals).

### 6. **Share Specific Times**
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
1. Use the date/time picker to select your proposed meeting time
2. Choose your office from the dropdown
3. Click "Apply" to see the time across all zones
4. Check the work hours indicators - green badges mean good timing!
5. Share the URL with your team

### Quick Time Check
- Just visit the site to see current time across all offices
- Green badges show who's currently in work hours
- Your nearest office is automatically highlighted

### Planning Async Communication
- Check the work hours indicators before sending messages
- Avoid purple (night) and blue (weekend) unless urgent
- Use yellow (early/evening) with caution
- Share a URL with a specific time to propose a meeting

### Before Sending a Slack Message
Just glance at the badges:
- **Green**: Go ahead, they're working
- **Yellow**: They might be available
- **Purple**: Send async, they'll respond later
- **Blue**: It's the weekend, wait until Monday

## 💡 Tips

- **Bookmark it** - Add to your browser bookmarks for quick access
- **Pin the tab** - Keep it open during your workday
- **Use the pickers** - Easier than manually editing URLs
- **Share URLs** - Send the link with your proposed time
- **Check the colors** - Respect work-life balance across timezones
- **No installation needed** - It's just a web page, works everywhere

## 🛠 Technical Details

- Fully client-side (no data collection)
- Works on mobile and desktop
- Updates every second when showing current time
- Respects browser timezone settings
- Uses Intl.DateTimeFormat API for accurate timezone conversion
- Native date/time pickers for easy interaction

---

**Questions or suggestions?** Feel free to reach out!

**Made with** ☕ **by Copilot with guidance from Simão**
