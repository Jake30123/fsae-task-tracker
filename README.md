# OEM Fabrication Tracker

A real-time task tracking dashboard for Olin Electric Motorsports (OEM) fabrication team.

![OEM Logo](oem-logo.png)

## Setup

1.  Clone the repository.
2.  Copy `firebase-config.example.js` to `firebase-config.js`.
3.  Add your Firebase API keys to `firebase-config.js`.

> **Note:** `firebase-config.js` is in `.gitignore` to keep your API keys private.

## How to Run

To run the application locally while connecting to the live Firebase database:

**Option 1: Using Node.js (Recommended)**
This avoids "file://" protocol issues with some browsers.

```bash
npm start
```
Then open [http://localhost:8080](http://localhost:8080) in your browser.

**Option 2: Simple File Open**
You can often just open `index.html` directly in your browser.

## Features

### General
- **Real-time Sync**: Updates appear instantly for all users via Firebase.
- **Mobile Friendly**: Designed for use on shop tablets and phones.
- **OEM Branding**: Custom color palette (blue, yellow) with Space Grotesk/Space Mono fonts.

### Member Portal
- **My Tasks**: View and manage tasks assigned to you.
- **Quick Status Updates**: Change task status directly from task cards.
- **Open Task Pool**: Browse and pick up unassigned tasks.
- **Subteam Filter**: Filter the open task pool by subteam.

### Lead Portal
- **Project Manager View**: PMs (Jake Hamilton, Alyssa Aranda) see all 5 subteam charts.
- **Subteam Lead View**: Leads see only their subteam's tasks and members.
- **My Assigned Tasks**: Leads can view their own personal tasks in addition to the master list.
- **Master Task List**: Full table view of all tasks with filtering.
- **Open Task Pool**: Filterable list of unassigned tasks.
- **Team Management**: Add/remove members and promote/demote leads.
- **Workload Charts**: Visual breakdown of tasks by status and member.

### Task Management
- **Due Dates**: Set due dates with overdue highlighting (red border + text).
- **Designer Field**: Track who designed each part.
- **PDF Drawings**: Link to external drawing files.
- **Quick Delete**: Remove tasks directly from the modal.

## Tech Stack

- **Frontend**: HTML, JavaScript, Tailwind CSS (CDN)
- **Backend**: Firebase Firestore (real-time database)
- **Fonts**: Space Grotesk (headings), Space Mono (monospace)
- **Charts**: Chart.js

## Subteams

- Drivetrain
- Suspension
- Accumulator
- Cockpit
- Aero
- General

## Contributing

1. Create a feature branch from `main`.
2. Make your changes.
3. Test locally with `npm start`.
4. Submit a pull request.
