# Rainy Exam Countdown

A cozy countdown app for exams and appointments, set in an animated rainy evening.

**Demo:** (https://wirwar14.github.io/oblig3_3650/)

## What it is and why I made it

Exam season is stressful, and it's easy to lose track of how much time is left. Rainy Exam Countdown shows a live clock and a countdown to every exam and appointment you add. The calm rainy background, rain sounds and gentle quotes make it a nice page to keep open while you study.

## Features

- **Live clock** that updates every second.
- **Countdowns** in days, hours, minutes and seconds for every exam and appointment. The next one is marked **NEXT**, items less than 3 days away are highlighted, and finished ones show "Done".
- **Add and remove** exams and appointments. Each item has a type, a title, optional details, a date and a time.
- **Filter** the list to show all items, only exams or only appointments.
- **Saves automatically** in the browser (localStorage), so your list is still there next time.
- **Animated background:** rain, ripples on the pond, flickering lanterns, a boat that rocks, and a cat that bobs in the water and blinks.
- **Five rain types**, each with its own look and sound: glass roof, anime rain, drizzle, downpour and classic.
- **Rain sounds and calm music**, all generated in code with the Web Audio API, so there are no audio files. The glass-roof rain is a dense, steady stereo downpour with long, rolling thunder, like a sleep-sounds recording.
- **4 rain sounds to choose from** in a menu: Gentle rain, Rainy evening indoors, Dripping garden and Thunder on the glass roof. The sound is chosen separately from how the rain looks.
- **"Only rain" switch** that turns off the music, heartbeat and clock tick, so you hear just the rain and thunder.
- **Gentle quotes and proverbs** that change every 20 seconds. Click the quote to see the next one.
- **Watch mode** that hides the content so you can just watch the rain.
- Works on both desktop and phone.

## How to run it

It's a single file with no installation. Download `index.html` and open it in Chrome, Edge or Firefox. Click anywhere on the page to start the sound, because browsers don't allow sound before you interact with the page.

## How I used AI

I built the app with **Claude** (Anthropic) by describing what I wanted in plain language, one step at a time. Claude wrote the code, and I tested every version in the browser and asked for changes.

How the app developed:
1. A simple exam countdown with a live clock.
2. Spooky sounds and a "sense of doom", then a darker, gloomier look.
3. A blue, more melancholic theme with rain and sad piano music.
4. Continuous rain sounds and a rainy-window background.
5. Several background styles (cottagecore, an old-cartoon look, a painted countryside), and finally an animated version of a rainy pond picture.
6. Different rain types, each with its own sound, including heavy rain on a glass roof.
7. A calmer tone: a new name, no emojis, gentle quotes instead of gloomy ones, and support for appointments as well as exams.

## Testing and improvements

| Problem I found | What we changed |
|---|---|
| No sound played when the page opened | Browsers block sound until you click, so the sound now starts on your first click, and there's a button to turn it on and off |
| I couldn't tell if the sound worked | Tested each sound on its own from the browser console |
| Text was hard to read on top of the busy background | Added a darker, slightly blurred panel behind the clock and the quotes |
| The title wrapped and the background was cropped badly on phones | Made the title smaller on narrow screens and framed the background so the cat stays in view |
| The cat and the boat were hidden behind the content | Added a "Watch the rain" button that hides the content |
| Adding and removing didn't work in Claude's preview window | The preview blocks forms and pop-ups. In a normal browser it works, so I tested it there |
| Every rain type sounded the same | Gave each rain type its own sound, with a smooth crossfade when you switch |
| I didn't like the rain sounds | Added a menu of different rain sounds made with softer, warmer noise. I tried about 20 and kept the four I liked best. Their volume is evened out so switching doesn't jump in loudness |
| The glass-roof rain sounded like separate ticks, not like a real recording of heavy rain | Compared it with a YouTube recording of rain and thunder on a glass roof, then changed it to a dense stereo wash, made the thunder long and rolling, and added an "Only rain" switch |

I also tested on desktop and phone screen sizes, added and removed items, reloaded the page to check that the list was saved, and checked the browser console for errors.

## Built with

- HTML, CSS and JavaScript in one file
- Canvas for the animation
- Web Audio API for all the sound
- Google Fonts: IM Fell English and Special Elite

## Credits

- **Background picture:** [say where it comes from, e.g. "generated by me with (name of the AI image tool)"]
- **Quotes:** old proverbs and old texts (Ovid, Laozi, Heraclitus, Aesop, A. A. Milne and others)
- **Code:** written with Claude, directed and tested by me
