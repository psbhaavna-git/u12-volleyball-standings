# U12 Volleyball Standings - PSR Power League

Live standings tracker for U12 teams in the Puget Sound Region Volleyball Power League.

**[View Live Standings]([https://yourusername.github.io/u12-volleyball-standings](https://psbhaavna-git.github.io/u12-volleyball-standings/index.html))**
## About

This website displays the current standings and schedule for all U12 teams competing in the PSR Power League. The site features:

### Standings Page (index.html)
- ✅ All 51 U12 teams with current rankings
- 🏆 Visual highlights for top 3 teams (gold, silver, bronze)
- 🔄 Auto-refresh timer (60 seconds)
- 📱 Mobile-responsive design
- ⏰ Last updated timestamp

### Schedule Page (schedule.html)
- 📅 Complete U12 Power League schedule
- 🎯 Visual timeline with past, current, and upcoming events
- 🔗 Direct links to AES for live schedules
- ℹ️ Important information about gate fees and roster requirements

## Data Source

Standings data is sourced from the official [PSR Volleyball Power League page](https://www.psrvb.org/power-league).

**Note:** Standings are typically updated every Tuesday following each play date.

## How to Update Standings

When new standings are posted (check the [PSR website](https://www.psrvb.org/power-league) on Tuesdays after play dates), follow these steps:

### Option 1: Manual Update (Easiest)

1. Download the latest U12 standings PDF from https://www.psrvb.org/power-league
2. Open `index.html` in a text editor
3. Find the `standingsData` array (around line 245)
4. Update the team rankings and points to match the new PDF
5. Save the file
6. Upload to GitHub (drag & drop in the repository, or commit via Git)

### Option 2: Using Git Command Line

```bash
# Clone the repository (first time only)
git clone https://github.com/yourusername/u12-volleyball-standings.git
cd u12-volleyball-standings

# Make your edits to index.html
# Then commit and push:
git add index.html
git commit -m "Update standings for PL#2"
git push
```

### Example Data Format

The standings are stored in this format inside the JavaScript:

```javascript
const standingsData = [
    { rank: 1, team: "PJVBC 12 National", code: "g12puyal1ps", points: 715.00 },
    { rank: 2, team: "Ignite 12 Red", code: "g12ignit1ps", points: 700.00 },
    // ... more teams
];
```

## Power League Schedule 2026

- **Jan 3** - U12 Seeding Day
- **Jan 24** - PL#1 U12
- **Feb 8** - PL#2 U12
- **Mar 1** - PL#3 U12

## Technical Details

- **Technology:** Pure HTML, CSS, and JavaScript (no dependencies)
- **Hosting:** GitHub Pages (free)
- **Auto-refresh:** Page updates display every 60 seconds
- **Browser Support:** All modern browsers (Chrome, Firefox, Safari, Edge)

## Future Enhancements

Possible improvements:
- [ ] Automated data fetching from PSR website
- [ ] Historical standings comparison
- [ ] Team search/filter functionality
- [ ] Points progression graphs
- [ ] Mobile app version

## Contributing

Feel free to submit issues or pull requests to improve the standings tracker!

## License

This project is open source and available under the MIT License.

## Contact

For questions about the Power League itself, visit [PSR Volleyball](https://www.psrvb.org/power-league).

For technical issues with this website, please open an issue on GitHub.

---

**Last Updated:** February 8, 2026  
**Current Standings:** PL#1 (as of January 26, 2026)
