# ConScribe

**Convention Scheduler for Tabletop Gaming Events**

*by DreamGlyph Studios LLC*

ConScribe is a scheduling and team management tool built for tabletop gaming convention organizers. Plan your game schedule, coordinate GMs and Event Organizers, and give your staff mobile access to real-time shift information.

---

## Table of Contents

- [Installation](#installation)
- [Getting Started](#getting-started)
- [Managing Your Team](#managing-your-team)
- [Game Library](#game-library)
- [Scheduling Games](#scheduling-games)
- [Schedule Views](#schedule-views)
- [Exporting & Sharing](#exporting--sharing)
- [Access Codes & Mobile App](#access-codes--mobile-app)
- [Group Collaboration](#group-collaboration)
- [Convention Settings](#convention-settings)
- [Auto-Updates](#auto-updates)
- [Tips & Shortcuts](#tips--shortcuts)

---

## Installation

### Desktop (Windows)

Download the latest release from the [Releases](https://github.com/DreamGlyphStudios/ConScribe-Releases/releases) page:

- **ConScribe-Setup-x.x.x.exe** — Standard installer (recommended). Installs to your system and receives automatic updates.
- **ConScribe-Portable-x.x.x.exe** — No installation required. Run from any folder or USB drive.

**System requirements:** Windows 10 (64-bit) or later.

### Mobile Companion (Android)

Download the latest APK from the [Releases](https://github.com/DreamGlyphStudios/ConScribe-Releases/releases) page and install it on your Android device.

> **Note:** iOS support is coming soon.

The mobile app is free and designed for Event Organizers (EOs) to view their convention schedules on the go. It requires an access code generated from the desktop app.

---

## Getting Started

### 1. Create Your Account

When you first launch ConScribe, you'll see the login screen:

- **Sign In** with an existing email and password
- **Sign Up** to create a new account (provide a display name, email, and password)
- **Forgot Password?** to receive a password reset email

### 2. Welcome Wizard

On your first login, a welcome wizard walks you through ConScribe's key features:

1. **Welcome** — Overview of what ConScribe does
2. **Schedule Games** — How the scheduling system works
3. **Team Coordination** — Managing your GMs and EOs
4. **Mobile Companion** — How EOs access their schedules on the go

Click **Create Your First Convention** to get started, or skip to explore on your own.

### 3. Create a Convention

Click the **Add Convention** button in the sidebar to create your first convention:

- **Convention Name** (required)
- **Year** (defaults to the current year)
- **Location**

Your new convention appears in the sidebar and is ready for scheduling.

### 4. Configure Your Settings

Open **Settings** (gear icon in the header) to configure your convention:

- **Opening Time** — When your earliest games can start (6 AM - 12 PM)
- **Closing Time** — When your latest games should end (5 PM - 11 PM)
- **Time Slot Interval** — 1 hour or 30-minute scheduling increments
- **Buffer Time** — Turnaround time between GM sessions (none, 30 min, or 1 hour)
- **Tables/Locations** — Add tables individually or in groups (e.g., "Table" x 10 creates Table 1 through Table 10). Reorder with the up/down arrows.

---

## Managing Your Team

Open the **Team Members** panel (people icon in the header) to manage everyone involved in your convention. The Team panel has three tabs:

### Roster

Your master list of all team members across all conventions.

- **Add Member** — Name, email, phone, Discord handle, preferred systems, default max hours, and status (Active, Pending, or Inactive)
- **Edit/Delete** — Click any member to update their info, or remove them entirely
- **Import** — Bulk import team members from a CSV or Excel file (see [Importing Data](#importing-data))

### Convention Roles

Assign roles to team members on a per-convention basis. Select a convention from the dropdown, then check the roles for each person:

| Role | Description |
|------|-------------|
| **GM** | Game Master — runs games. When checked, a GM Hours field appears for scheduling limits. |
| **EO** | Event Organizer — oversees the gaming area during shifts |
| **Setup** | Helps with pre-convention setup |
| **Breakdown** | Helps with post-convention teardown |
| **Admin** | Convention administration |
| **Volunteer** | General volunteer |

A single person can hold multiple roles (e.g., someone can be both a GM and an EO).

### EO Shifts

Schedule when each EO is on duty. Select a convention, then:

- Choose an **EO** from the dropdown (filtered to members with the EO role)
- Pick the **Day**, **Start Time**, and **End Time**
- Click **Add** to create the shift

EO shifts appear on the grid view as colored columns alongside the game schedule.

---

## Game Library

Open the **Game Library** (dice icon in the header) to manage your catalog of games.

### Adding Games

Click **Add Game** and fill in:

- **Title** (required)
- **System** — The game system (e.g., D&D 5e, Pathfinder, Call of Cthulhu)
- **Level** — Experience level or tier
- **Type** — Adventure, Horror, Dungeon Crawl, Intrigue, One-Shot, Campaign, Tournament, or Other
- **Duration** — 0.5 to 12 hours
- **Max Players** — 1 to 20
- **Description** — A summary for players and GMs
- **Colors** — Pick custom light and dark theme colors for the schedule grid

### Convention Availability

Check the box next to each convention to mark a game as available for scheduling at that event. Only available games appear when scheduling.

### Importing Data

Both the Game Library and Team Roster support importing from **CSV** or **Excel** (.xlsx/.xls) files:

1. **Select File** — Choose your spreadsheet. ConScribe shows the file name, row count, and column count.
2. **Map Columns** — Assign each column from your file to a ConScribe field. Required fields are marked with an asterisk. Use "Skip" for columns you don't need.
3. **Preview** — Review the first 10 rows of mapped data. Any validation errors are listed.
4. **Import** — ConScribe imports your data with a progress bar. A final summary shows how many rows were imported, skipped (duplicates), or had errors.

---

## Scheduling Games

Click any empty slot in the Grid View, or use the **Add Game** button to open the scheduling dialog:

1. **Select a Game** — Choose from your convention-available library. Fields auto-fill from the library entry (title, level, system, duration, colors).
2. **Assign a GM** — Pick from team members with the GM role. Their contact info (email, phone, Discord) is displayed for reference.
3. **Pick Day & Time** — Select the day and starting time slot.
4. **Assign a Table** — Choose from your configured tables/locations.
5. **Set Status**:
   - **Tentative** — Penciled in, not yet confirmed
   - **Confirmed** — Locked in the schedule
   - **Cancelled** — Removed from active schedule but kept on record
6. **Add Notes** — Optional notes for special requirements.

### Conflict Detection

ConScribe automatically checks for scheduling conflicts when you save a game:

- **GM Conflict** — The assigned GM is already running a game at the same time
- **Table Conflict** — Another game is scheduled at the same table and time
- **Buffer Conflict** — The GM doesn't have enough turnaround time between sessions

You'll see a warning describing the conflict. You can choose to save anyway (override) or go back and adjust.

---

## Schedule Views

Switch between three views using the tabs at the top of the schedule:

### List View

A compact, sortable table of all scheduled games showing:

- Game title and status badge
- Description (abbreviated)
- GM name
- Day, time, and duration
- Table assignment
- Level and system

Click any row to edit the game.

### Grid View

A visual matrix with **days as columns** and **time slots as rows**:

- **Game cells** are color-coded using each game's custom theme colors and show the title, level, and GM name
- **EO columns** appear alongside tables, showing who is on shift at each time (displayed as vertical text with distinct colors)
- **Buffer slots** are visually marked when buffer time is configured
- The grid automatically crops to the relevant time range of your scheduled games

Click any game cell to edit it, or click an empty cell to schedule a new game.

### GM View

A card-based layout showing one card per GM:

- **Workload bar** — Visual indicator of scheduled hours vs. maximum hours. Turns red if a GM is overbooked.
- **Game list** — All games assigned to that GM with title, level, day, time, and duration
- **Game count** and total scheduled hours

Click any game on a card to edit it. This view is useful for spotting overloaded or underutilized GMs at a glance.

---

## Exporting & Sharing

Open the **Export** panel (file-export icon in the header) to share your schedule:

### Print Schedule

Generates a printable grid view of your full schedule:

- Tables and EO shifts as columns
- Time slots as rows
- Games displayed with title, level, and GM name
- Opens in a preview window with a print button

### GM Schedules

An interactive view for sharing schedules with your GMs:

- **Filter by GM** and **filter by Day**
- Each GM's card shows their full schedule with game details: day, time, duration, title, table, max players, status, and assigned EO
- **Copy All** — Copies a plain-text summary of all games to your clipboard
- **Copy for Email** — Generates a pre-formatted, personalized message for each GM (e.g., "Hi Sarah, here is your schedule for GameCon 2026...")

---

## Access Codes & Mobile App

### Generating Codes (Desktop)

Open the **Access Codes** panel (key icon in the header):

1. Ensure you have EOs assigned to shifts for the convention
2. Click **Generate Codes** — ConScribe creates a unique 8-character code (format: XXXX-XXXX) for each EO
3. **Copy** each code and share it with the corresponding EO (via email, Discord, text, etc.)
4. Codes can be **Revoked** individually or all at once if needed

### Using the Mobile App (EO)

Your Event Organizers use the free ConScribe mobile companion:

1. **Enter Code** — Open the app and type in the access code you provided
2. **Schedule View** — See the full convention grid for each day, with color-coded games and EO shift columns. Tap any game for details.
3. **My Shifts** — See only the shifts assigned to them, organized by day. Each shift shows which games are running during that time.
4. **Game Details** — Tap any game to see the full details: title, status, schedule, table, level, system, max players, description, and GM contact info (with tappable links for email, phone, and Discord).

The mobile app works offline — schedules are cached locally and refresh automatically when connectivity is available. A "Last updated" banner shows how fresh the data is, and pull-to-refresh forces a sync.

EOs can save multiple convention codes and switch between them from the convention list.

---

## Group Collaboration

ConScribe supports team collaboration through Groups. Open the **Group Management** panel from your profile area.

### Creating a Group

1. Go to the **Create Group** tab
2. Enter a **Group Name**
3. Click **Create** — You'll receive a join code to share with your team

### Joining a Group

1. Go to the **Join Group** tab
2. Enter the 6-character **Join Code** from your group's owner
3. Click **Join**

### Managing Members

The group owner can manage member permissions from the **Members** tab:

| Permission | What It Allows |
|------------|----------------|
| **Manage Team** | Add, edit, and delete team members |
| **Schedule Games** | Add, edit, and delete games from the schedule |
| **Manage Conventions** | Change convention settings (times, tables, buffer) |
| **Access Codes** | Generate and revoke EO mobile access codes |
| **Export** | Export and print schedules |
| **API Access** | Generate API tokens for bulk import/export operations |

The owner can also:

- **Transfer Ownership** — Hand the group over to another member (you become a regular member)
- **Remove Members** — Remove someone from the group
- **Regenerate Join Code** — Invalidate the old code and create a new one
- **Delete Group** — Permanently delete the group and all shared data

### API Access

Members with the **API Access** permission can use ConScribe's bulk endpoints for automated data management. From the **Group Info** tab, copy your API token, base URL, and group ID for use with external tools and scripts.

---

## Convention Settings

Access settings via the **gear icon** in the header. Settings are per-convention.

### Time Configuration

| Setting | Options | Description |
|---------|---------|-------------|
| **Opening Time** | 6 AM - 12 PM | Earliest schedulable time slot |
| **Closing Time** | 5 PM - 11 PM | Latest schedulable time slot |
| **Time Interval** | 1 hour / 30 min | Granularity of your time slots |
| **Buffer Time** | None / 30 min / 1 hour | Required gap between a GM's consecutive sessions |

### Table Management

- **Add Group** — Enter a prefix (e.g., "Table") and count (e.g., 8) to create Table 1 through Table 8
- **Add Custom** — Add a single table with a custom name (e.g., "Main Stage", "VIP Room")
- **Reorder** — Use the up/down arrows to change table display order
- **Delete** — Remove tables you no longer need (minimum 1 required)

---

## Auto-Updates

ConScribe checks for updates automatically when you launch the app. If a new version is available:

1. A banner appears at the top: **"ConScribe x.x.x is available"**
2. Click **Download** to start the update (or **Later** to dismiss)
3. A progress bar shows download progress
4. Once downloaded, click **Restart Now** to apply the update, or it will install automatically the next time you close and reopen ConScribe

---

## Tips & Shortcuts

- **Theme Toggle** — Click the moon/sun icon in the header to switch between light and dark mode
- **Change Password** — Click the lock icon in the header to update your password
- **Help Menu** — Access the Privacy Policy and API Documentation from the Help menu in the title bar
- **Convention Switching** — Click any convention in the sidebar to switch between events
- **Quick Schedule** — Click empty cells directly in the Grid View to schedule a game at that day/time/table

---

## Support

For questions, bug reports, or feature requests, visit the [ConScribe Issues](https://github.com/DreamGlyphStudios/ConScribe-Releases/issues) page.

---

*Copyright 2026 DreamGlyph Studios LLC. All rights reserved.*
