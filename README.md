# Kids' Chore Chart for a Chromebook

One full-screen page with a column for each kid (up to 4). Each kid has their own world and animal (Bug Garden, Rainbow Unicorn or Dino Valley), chores, stars, levels, month view and prize box. Version 3.3.0.

## Files

- `index.html` is the whole app.
- `sw.js` lets it open without internet after the first visit.
- `manifest.webmanifest` and the icons let the Chromebook install it as an app.
- `version.txt` tells the app when a new version is online.

The code holds no names or schedules. Kids' details are typed on the Chromebook during setup and stay there.

## Put it online (GitHub Pages)

1. Make a public repository, for example `chore-chart`, and upload every file in this folder.
2. Settings > Pages > Deploy from a branch > `main` / root > Save.
3. A few minutes later the app is at `https://YOUR-USERNAME.github.io/chore-chart/`.

## Set up the Chromebook

1. Open the address in Chrome. Setup asks how many kids, each kid's name, world, age group (for starter chores) and, if you like, a school with a daily XP goal; then a 4-digit parent PIN.
2. Install it: Chrome menu > Cast, save and share > Install page as app (or the install icon in the address bar). Open it from the launcher.
3. Tap the chart once: it goes full screen (Parents > Family > Screen to change that) and sounds are switched on.
4. Chromebook Settings:
   - System preferences > Power > Charging optimization: choose Charge limit (80%) if your model offers it, so a Chromebook that is always plugged in keeps a healthy battery.
   - System preferences > Power: while charging, set the idle action to turn off the display. The app keeps the screen on during the day and lets it turn off at night (bedtime to morning).
   - Apps > Restore apps on startup: Always restore, so the chart comes back after the Chromebook restarts for an update.
5. Use a separate Google account for the wall Chromebook, with none of your email or files in it, because kids can swipe out of any app.

## How it works

- Chores belong to a part of the day: Morning, Evening or Night. No clock times on chores. The part the kid is on is outlined.
- When a part starts (Parents > Family > Parts of the day; defaults 7:00 AM, 3:30 PM and 6:00 PM), each kid with chores in it hears a reminder. It repeats every 2 minutes, up to 3 times (once, twice or 3 times in Parents > Family > Reminders and sounds), and stops for a kid once they check something in that part.
- Quieter: potty reminders can be a soft chime without words. The speaker button at the top mutes all sounds for an hour (parent PIN); tapping it again turns them back on. Reminders still glow while muted.
- School (optional, per kid): one item in its own School part (default 8:30 AM), showing its daily XP goal, for example "120 XP goal", and "120 XP completed" once checked.
- Potty (optional, per kid; on for ages 2 to 3): a Potty button with the next time. The first reminder plays when the morning starts, then every 2 hours after the last potty event (1 to 3 hours in settings) until bedtime. "I went" logs a trip and earns a star for the prize box. A trip counts once every 20 minutes.
- Potty log (parents): under a kid's tab, Fix a day logs trips, tries and accidents with a time; tries and accidents never show on the kids' screen. The Potty card shows the last 7 days and how long after the last trip accidents tend to happen, with a suggestion when a shorter gap may help.
- Yesterday: a button in each column opens the day before, to check chores the kid forgot to tap. It goes back to today after a minute. Parents can turn it off or require the PIN (Parents > Family > Yesterday).
- First and Then: at the top of each column, the chore to do now and the one after it, in the order of the chores list, inside the part of the day the kid is on. After the last chore of a part, Then shows the next part and when it starts. When potty time comes, Potty is First, with its I went button.
- Steps: a chore can have up to 8 steps with pictures (starter steps for Wash hands & face, Wash hands, Brush teeth, Get dressed and Toys away). Tapping the chore opens its steps in that kid's column: a list with check circles, or one step at a time with a big Done button (Parents > a kid's tab). Each step fills the chore; the last one checks it. Steps can be read out loud.
- Tap a chore without steps to check it. To undo, press and hold a finished chore (or a checked step) for a second; the tile fills while it is held, and a quick tap only shows "Hold to undo". A chore with steps loses only its last step. Toddler mode says the chore's name again on a quick tap. Several kids can tap at the same time.
- Must go in order (off by default, per kid): later chores in a part stay grey until the earlier ones are done.
- Big view: tapping a kid's name makes that column big, and the others shrink to strips with their stars and First chore. It goes back when the name is tapped again, or after 2 minutes without a tap (1 to 5 in settings); the countdown turns amber for the last 15 seconds. Not on phones.
- Chore columns: by part of the day (default), all together, or toddler mode (just this part of the day, very big pictures).
- Each chore, and school, can run every day or only on some days.
- A day with everything done is 100 XP. The kid's animal grows a size every 5 levels and changes form at levels 20, 40, 60 and 80 (caterpillar to blue butterfly, foal to rainbow unicorn, egg to great dinosaur). Every 10 levels brings a new rank and a full-screen celebration; level 99 has a finale.
- My month and Prizes open inside that kid's column, so the others keep going. A prize needs the parent PIN, and then the parent picks Given now or Later. A prize given later stays owed: it shows under Coming up in the kid's prize box and under Parents > Family > Prizes owed (the Family tab shows a count) until it is marked given.
- Family goal: every kid's chore stars this week (Monday to Sunday) count toward one shared reward, shown at the top of the chart. Automatic goal: 80% of the kids' weekly goals added up, or set your own. Days off lower it. Reaching it plays a celebration in every column once a week and puts the reward under Prizes owed.
- Bedtime to morning: a dark night screen, no sounds, no screensaver.
- Photo screensaver after a few idle minutes (Parents > Family). Photos stay on the Chromebook.
- Parents > a kid's tab: chores by part of the day and their days, school, potty schedule, fix a day (including potty trips), days off (for one kid or all), prize box, goal and reward, levels.

## Updating

Upload the new files to the repository. Within a few hours the Parents button shows a red dot; Parents > Family > App > Update now loads the new version. Data stays as long as the address stays the same. Chores from older versions that had clock times move to Morning (before noon), Evening (noon to 6 PM) or Night.

Updating to 3.3 from an older version: each kid with morning chores gets Wash hands & face at the start of the morning, the morning is put in the order Wash hands & face, Brush teeth, Get dressed, then the rest, and the chores that have starter steps get them. Change or remove any of it under each kid's tab. A backup from an older version gets the same changes when it is restored.

## Backup and PIN reset

- Parents > Family > Backup > Copy backup (paste it into a note or an email to yourself) or Download backup file (then move it to Google Drive, since a reset clears Downloads). Restore takes it back. Photos and the PIN are not included. A backup from the one-kid tablet chart adds that kid.
- After 30 days without a backup, a reminder with a Back up now button shows at the top of Parent settings.
- Forgot the PIN: open the address with `#reset-pin` at the end, set a new PIN.

## Good to know

- The PIN keeps kids out of settings. It is not strong security.
- Kids can check yesterday's chores without a grown-up unless you turn on the PIN for it.
- Clearing Chrome's site data for this address erases the chart unless you have a backup.
- Reminders play only while the app is open. After the app restarts, sounds come back with the first tap.
- Folded flat (tablet mode), ChromeOS shows the same picture on any connected monitor. Leaving a mouse plugged in switches it to desktop mode while folded.
