# Information Center

## Purpose

The Information-Center presents details of interesting questions. Ideally in a single "at-a-glance" view.

Here are some initial dynamic questions I want answered:

- Who is home?
- Is the Clothes Washer running?
  - Estimate of remaining time?
- Is it an okay time to start the dryer?
- Timezone and current-time where friends
- Recent events of interest:
  - Recent times external doors have been opened/closed
  - Recent times door-bell has been rung.
  - Who was the last to enter/leave the house
    - Not sure how to detect this
- Upcoming events of common interest
  - Movie release/watch plans
  - Flight arrivals
- Group "whiteboard" chat
  - Shares things like:
    - Need clothes soap soon
    - Trash needs to be taken out.
    - Put recycling bin out soon.
  - Perhaps a feed from a shared FB chat.
- MQTT event log
  - Recent MQTT messages, maybe filtered, or just a specific subscription.
- Is there mail in the box?
  - Time of arrival?
  - Time of removal?
- Has the fridge door been open for "too long"?
  - Perhaps send an audible alert

It may also include "static" information:

- WiFi info
- Links to interesting things, e.g.
  - D&D Manuals
- Power, water consumption history

It may offer some limited controls:

- Turn lights on/off (e.g. WeMo)
- Lock/unlock the front door

## Approaches

### Internal web site

Perhaps a VM running a .NET Core site.

## Concerns

- Perhaps some options/information should only be available to those internal to the network. Such as unlocking the front door.
- A "whiteboard" functionality would benefit from authenticating users. Perhaps a third-party plug-in.

## Other Resources

[Home Digital Info Center](https://www.raspberrypi.org/forums/viewtopic.php?t=188560)