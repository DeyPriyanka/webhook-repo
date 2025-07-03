"Final test push"

# GitHub Webhook Receiver & Activity Feed

This project is a Flask application built for the TechStax Developer Assessment Task. It's designed to receive GitHub webhooks for 'Push', 'Pull Request', and 'Merge' events. It processes these events, stores the relevant information in a MongoDB database, and displays them on a simple, auto-refreshing UI.

## Features

- **Webhook Receiver:** A Flask endpoint at `/webhook` listens for POST requests from GitHub.
- **Data Processing:** Parses payloads for Push, Pull Request (opened), and Pull Request (merged) events to extract key details.
- **MongoDB Integration:** Stores formatted event data in a MongoDB collection.
- **Real-time UI:** A simple frontend at the root URL (`/`) polls an API endpoint (`/events`) every 15 seconds to display the latest repository events.

---

## Setup and Installation

Follow these steps to get the application running locally.

### 1. Clone the Repository

```bash
git clone https://github.com/DeyPriyanka/webhook-repo.git
cd webhook-repo
```
