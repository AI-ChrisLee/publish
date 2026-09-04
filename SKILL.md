---
name: publish
description: Use this when the cut is finished and the video needs its YouTube listing. The founder says "set this video up on YouTube", "write the listing", "do the description and the chapters", "/publish", and later "it is live" with the URL. It copies the title the package locked, writes the description with one call to action, reads the chapters off the finished cut, and hands back the tags and the end screen for the founder to type into YouTube Studio. When the upload is live it appends one row to squad/content-log.md, the file the Sunday read counts. It never uploads, never publishes and never schedules.
---

# Publish

The cut is finished. **Your work, in one line: turn the cut into a listing the founder
pastes into YouTube Studio, then log the one row that makes the video countable.** The
founder's part: the upload, the thumbnail, the paste, and their own hand on publish.

**You never publish.** No upload, no scheduling, no thumbnail, no tag typed into an
account, no end screen set for them. You write, they paste, they press the button. There
is no connector in this run and you never ask for one.

This skill runs in ANY founder's repo. `.claude/squad-roots.md` is the per-repo instance
file every member-run skill reads first (founder name, product word, the `week`,
`episodes` and `content log` paths), and its values win over the `squad/` paths below,
which are worked examples. A row reading "(none yet)" is an unanswered field, not an
override: the worked-example path stands until this run fills it. `<date>` is the week's
date, `YYYY-MM-DD`, the same one the package file carries.

## The modes, and how they are called

| Mode | The founder says | Beats |
|---|---|---|
| listing | "set this video up on YouTube", "write the listing", `/publish listing` | 0, 1, 2, 3 |
| live | "it is live" with the URL, "the video is up", `/publish live` | 4 |

## The run map (where you run, where you STOP)

| Beat | Mode |
|---|---|
| 0 THE SOURCES | AUTO: the package, the finished cut's captions, the script, the sales script's booking link. No package, or no title in it: **STOP**, the title is C2's |
| 1 THE TITLE | AUTO: the MAIN title copied out of the package, character for character |
| 2 THE DESCRIPTION | AUTO: one call to action, the hook line, the search paragraph, the chapters, the stack |
| 3 THE LISTING | AUTO: written and printed, then **STOP · GATE: the founder uploads, sets the thumbnail, pastes the listing, points the end screen, and presses publish or sets the hour** |
| 4 THE ROW | HUMAN INPUT: the live URL; then AUTO: one row appended to the content log |

The beat numbers ARE the step numbers below. Beat 3 is the only stop, and it is a real
one: everything after it happens inside the founder's own YouTube account, by hand.

**Resuming.** The rule keys on the OUTPUTS, never on a session's memory. Check them in
this order and continue at the first one missing.

| Missing or incomplete | Resume at |
|---|---|
| `squad/week/<date>-listing.md` does not exist | beat 0 |
| the listing exists and the founder has not said the video is live | nothing to redo, print the listing file and the by-hand list again |
| the founder gives a live URL and `squad/content-log.md` holds no row with that video id | beat 4 |
| a row with that video id is already there | done. Never write a second row for one video |

The last two rows are entered by the founder's word, never by a file: an upload happens
inside YouTube and leaves nothing on the laptop.

## The outputs (3 files, every run)

1. `squad/week/<date>-listing.md`: the title, the description whole, the chapter block,
   the tags and the end screen target. It is what the founder copies from at upload,
   which can be days after this run.
2. `squad/content-log.md`: ONE row appended per video, columns
   `date | title | link | video id`. The file with its header row when it does not exist.
   C6 reads every row on Sunday.
3. `.claude/squad-roots.md`: the `content log` row when it carries none. Nothing else in
   it touched.

Nothing else gets written. Never a spreadsheet, never a calendar, never the package file,
never the script, never the cut.

## Beat 0 · The sources

**Read these four, then say in one line what opened.**

| What | Where | What it gives |
|---|---|---|
| the package | `squad/week/<date>-package.md`, the latest (or `<date>-repackage.md` when this video was repackaged) | the MAIN title, the TEST line, and `episode:` naming the episode folder |
| the finished cut | the caption file (`.srt`) the cut wrote, or the cut's exported transcript | the real timings the chapters come from |
| the script | `03_SCRIPT.md` in that episode folder | the hook line and the tools named on camera |
| the sales script | `squad/sales.md` | the booking link, which is the one call to action |

**No package file, or a package with no locked title: STOP on one line.** The title is
`the-proven-package`'s and this run never makes one up.

**No caption file and no exported transcript: ask for one and stop.** Never guess a
timestamp, and never take chapters off the script; the script's timings were estimates
the cut moved.

**No `squad/sales.md`, or a booking link still reading `[BOOKING LINK]`:** write the
description with no call to action, say so in one line, and tell the founder the link is
G6's and the listing is rewritten once it exists.

## Beat 1 · The title

Copy the MAIN title out of the package, character for character. **Never re-title.** It
was locked with the thumbnail it is paired with, and the founder already changed every
word that did not sound like them.

A founder asking for a different title is asking for `the-proven-package`, not for this.
Say that in one line and change nothing.

## Beat 2 · The description

This order, no improvising:

1. **ONE call to action at the top**, as `Phrase : URL`. The booking link from
   `squad/sales.md`, as a plain URL.
2. A hook line.
3. One plain paragraph for search, in the words a buyer would type.
4. The `CHAPTERS` block.
5. `THE STACK`: the tools named in the video, each a plain link.

**One call to action, so one opt-in link.** Two links maximum: the booking link, and the
one tool in THE STACK the video actually runs on. A STACK link is a tool link. It never
carries the call to action and it never gets a row of its own.

Plain URLs only. No tracked redirect, no minted link, no shortener.

No em dashes anywhere. This is outward-facing.

## Beat 3 · The listing, then stop

**Chapters, off the finished cut.** First chapter at `0:00` or YouTube throws out the
whole list. Three minimum, each at least 10 seconds, named for what is on screen at that
timestamp. A chapter that lies is worse than no chapter, so the name matches the section
that actually starts there.

**Tags and the end screen, as text.** Up to 15 tags, the words a buyer would search. The
end screen points at the next video in the series, or at the founder's best related
video. Both go in the file for the founder to type in Studio.

Write `squad/week/<date>-listing.md` with all of it and print it.

**Then STOP, and say plainly what is left, all of it by hand in YouTube Studio:**

- Upload the file, private if it is going out on a schedule.
- Add the caption file as the subtitle track.
- Set the thumbnail from the package, and read the package's own TEST line while it is
  open.
- Paste the title and the description.
- Type the tags, point the end screen.
- Press publish, or set the hour and let YouTube press it.

Never publish or schedule anything yourself, and never offer to.

## Beat 4 · The row

The founder comes back with the live URL, sometimes the same hour and sometimes the next
day.

Append ONE row to `squad/content-log.md`: `date | title | link | video id`. Today's date,
the locked title, the URL, and the id after `v=`. Create the file with that header row
when it does not exist, and add the `content log` row to `.claude/squad-roots.md` when it
carries none.

One row per video. Never a second row for a video id already in the file.

Then one line back: the row is what the Sunday read counts, and a video with no row is
invisible to it.

## Rules

- **Never send, never publish.** No upload, no schedule, no thumbnail, no tag typed into
  any account.
- **Never write a title.** The package locked it.
- **Never invent a timestamp.** Chapters come off the finished cut or the run stops.
- **Never a second call to action.**
- **Never price past what `squad/business.md` carries**, and never put a number, a claim
  or a tool in the description that the video does not carry.
- **Never invent a number, a name or a need**, and never paraphrase a quote from the
  script into something the founder did not say.
- **Never write to a spreadsheet, a calendar or an account.** This run touches two files in
  `squad/` and one roots row.
