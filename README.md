# FSAE Fabrication Task Tracker

A real-time task tracking dashboard for the FSAE fabrication team.

## Setup

1.  Clone the repository.
2.  Copy `firebase-config.example.js` to `firebase-config.js`.
3.  Add your Firebase API keys to `firebase-config.js`.

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
- **Real-time Sync**: Updates appear instantly for all users.
- **Role-based Views**: 
    - **Leads**: Can edit all tasks, manage roster, and view stats.
    - **Members**: Can view their tasks and pick up open tasks.
- **Mobile Friendly**: Designed for use on shop tablets and phones.
