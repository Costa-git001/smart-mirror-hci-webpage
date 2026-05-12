# Smart Mirror HCI Webpage

This project is an HCI CAT webpage that simulates a smart mirror interface using the device camera. The camera video is flipped horizontally so the user sees themselves as they would in a real mirror, while useful information appears as glanceable panels around the edges.

## Assignment Goal

Design a simple webpage that simulates a smart mirror for a home context. The interface supports:

- Live camera-based mirror simulation
- Visual display of useful information on the mirror
- Tap-based control through menu items and widgets
- Voice control/input
- Speech output from the mirror

## Main Smart Mirror Features

### 1. Time and Date

Time and date are the main default display because most people check a mirror while getting ready.

Example display:

```text
10:42 PM
Tuesday, 12 May 2026
```

Voice command:

```text
Mirror, what time is it?
```

Speech output:

```text
It is 10:42 PM.
```

### 2. Agenda / Calendar

Shows the user's daily schedule.

Example:

```text
Today's Agenda
13:00 - HCI Class
17:00 - Football Practice
20:00 - ADS CAT Revision
```

Menu item: `Agenda`

Tap interaction: tap `Agenda` to expand the full schedule.

Voice command:

```text
Show my agenda.
```

Speech output:

```text
You have three events today. Your next event is HCI Class at 1 PM.
```

### 3. Weather

Shows the current weather and a short forecast.

Example:

```text
Nairobi
22C | Cloudy
Rain expected later
```

Menu item: `Weather`

Tap interaction: tap the weather widget to show weather details.

Voice command:

```text
What's the weather today?
```

Speech output:

```text
Today is cloudy with a temperature of 22 degrees.
```

### 4. News Headlines

Displays only 2 to 3 short headlines so the mirror does not overload the user.

Example:

```text
Top News
- New AI tools launched
- Country's updated morning run in Nairobi
- Sports results today
```

Menu item: `News`

Tap interaction: tap a headline to expand a short summary.

Voice command:

```text
Show news.
```

Speech output:

```text
Here are today's top headlines.
```

### 5. Health / Wellness

Shows simple daily wellness reminders using mock data.

Example:

```text
Health
Water: 4/8 glasses
Steps: 3,200
Sleep: 6h 45m
Mood: Good
```

Menu item: `Health`

Tap interaction: tap to update water intake or mood.

Voice command:

```text
How is my health summary?
```

Speech output:

```text
You have walked 3,200 steps and slept for 6 hours and 45 minutes.
```

### 6. Reminders / To-Do List

Shows quick daily tasks.

Example:

```text
Reminders
- Submit HCI CAT
- Revise for ADS CAT
- Charge laptop
```

Menu item: `Reminders`

Tap interaction: tap a task to mark it complete.

Voice command:

```text
Show my reminders.
```

Speech output:

```text
You have three reminders today.
```

### 7. Fitness / Morning Routine

Gives the mirror a realistic home-use feel.

Example:

```text
Morning Routine
Done: Brush teeth
Done: Take breakfast
Next: Pack laptop
07:30: Leave by 7:30
```

Menu item: `Routine`

Voice command:

```text
Start my morning routine.
```

Speech output:

```text
Your next task is to pack your laptop.
```

### 8. Smart Home Controls

Simulates smart-home controls for a home smart mirror context.

Example:

```text
Smart Home
Lights: ON
Fan: OFF
Room Temp: 24C
```

Menu item: `Home`

Tap interaction: tap to turn lights or fan on and off.

Voice command:

```text
Turn on the lights.
```

Speech output:

```text
Turning on the lights.
```

## HCI Design Considerations

- Information is placed around the edges so the user's face remains visible in the mirror.
- Content is short and glanceable because mirror use is usually quick.
- Tap controls are large enough for easy use on touch screens.
- Voice commands support hands-free interaction while getting ready.
- Speech output improves accessibility and gives the interface a smarter feel.
- Mock data is used for weather, health, reminders, agenda, and smart-home controls because this is a student prototype.

## How to Run

Open `index.html` in a browser, or serve the folder locally:

```bash
python -m http.server 8080
```

Then open:

```text
http://127.0.0.1:8080/
```

Camera and microphone features require browser permission. Speech recognition support depends on the browser.
