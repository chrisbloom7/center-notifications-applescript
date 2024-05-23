# center-notifications-applescript

An AppleScript utility to move notifications to the center of the screen on wide displays.

## Why

### Short answer

Because ADHD

### Long Answer

I have adopted many tricks for combatting my ADHD over the years. A persistent problem for me is forgetting about upcoming events. One way I was able to stay ahead of this was by immediately adding events to my calendar (sometimes multiple calendars) and adding multiple default notifications for each to help them stick in my head.

Over time that trick and others become less effective, and I finally decided to get setup with medication to help. It's been great, literally life changing. I can lock in on a task and stay focused for hours. Aaaand that presents it's own problem, because now it's super hard to unfocus my attention when I need to switch contexts. So I had to come up new tricks to combat that: lots and lots of notifications from multiple sources.

When I work on my laptop I tend to miss less meetings because the notifications are in my field of vision and cover parts of the window I'm focused on. However, I'm less productive overall on my laptop so I tend to prefer working at my desk where I've got all my softare development tools including a widescreen monitor. The monitor is great for keeping multiple apps in the foreground - an editor, a couple browser windows with docs up, a terminal window, etc... Buuuuut.... It's so wide that the notifications are easy to ignore of my focus is on my primary app in the middle - they aren't in my way enough, and I've managed to train myself to tune out most audible alerts unless they are persistant and  annoying, which isn't an option on a lot of apps.

So we're here now. I have this script setup as a login item that runs in the background. On wide displays (> 2048 DPI) it will monitor for new notifications and reposition them to the center of the screen. Right in my way. Right over the thing I'm most likely focused in on. If I switch displays (like move to my laptop) it will reposition them to the top right corner where they usually appear.## Installation### Using Compiled App1. Download `Center Notifications on Wide Displays.zip`.
2. Uncompress the zip file.
3. Copy `Center Notifications on Wide Displays.app`  to your user's `~/Applications` folder.### From Source1. Download `Center Notifications on Wide Displays.scpt`.
2. Open the script with `/Applications/Utilities/Script Editor`. (It should be the default editor for scpt files.)
3. Click File -> Export...
4. Select your user's `~/Applications` folder for the destination.
5. Select "Application" for File Format and "Sign to Run Locally" for Code Sign. Leave all options unchecked.
6. Click Save.

## Setup

1. Copy the application to your user's `~/Applications` folder2. Open the app to trigger access control permissions requests. It should prompt to grant the application control of System Events and Accessibility features.3. Right-Click the icon in the task bar, select Options, Open at Login.