# Overview

Like in vim, there could be utility to operating a twitch stream in a variety of modes depending on the task. This
project aims to define useful twitch modes and implement them in a practical fashion that is conducive to live
programming among other things.

This project is mostly motivated by the need for something like "pomodoro mode" documented below which will likely be the MVP.

# Spec

## Modes

### focus mode

This mode is optimized for doing focused work in which the streamer can operate on a single thread of attention for an extended amount of time, conducive to tasks such as programming.

Optional timer with alert when timer expires and optional automatic mode change when timer expires.

### short break mode

this mode is used for intervals between focus mode. maybe it could do something like have a queue of all the messages received in chat since the last focus mode started.

### long break mode

for pooping and stuff

### Vibe mode

This mode is not optimized for anything and lets the streamer just sort of do whatever they want.

### Just chatting mode

This mode is optimized for interacting with chat.

### Pair mode

This mode is optimized for collaborating with 1 or more other individuals. Perhaps there's utility in there being a "streamer pair mode" in which another live streamer is the collaborator and another "chat pair mode" in which 1+ members of chat are involved.

### Leet code mode

Shows current problem on leetcode or something

## Stream UI

### Statusline

Like in vim the mode can be tracked by a "statusline" that runs along the bottom of the screen with the name of the mode and any relative state such as timers or messages. 

### Task stack

I often find myself setting aside an active task for another task that I'd like to complete first as many programmers do in the classic "yak shaving" paradigm. This bit of UI would create an actual stack data structure inspired widget in which the streamer could push and pop items from their command interface.

### Interactive stream overlay

Like cardboardlive.

In the MVP we'll likely just lean on displaying ! chat commands for displaying information that's too much for the status line but it would be nice if the user could interact with the statusline using their mouse to click links and hover for tooltip style info windows.

## API
