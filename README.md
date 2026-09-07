# Publish: install in 60 seconds

The listing half of an Execution Squad's content lane. The cut is finished; this turns it
into the title, description, chapters, tags and end screen you paste into YouTube Studio,
and it logs the one row that makes the video countable on Sunday.

It never uploads and it never presses publish. That stays your hand.

## What to bring

The package `the-proven-package` locked (the title comes out of it, never rewritten), the
caption file the cut wrote (the chapters come off the real timings), and
`squad/sales.md`, where your booking link lives. No booking link yet? The listing still
gets written, without a call to action, and you rerun it once the link exists.

## Run it

Drop this whole folder into `.claude/skills/` as `publish`, quit and reopen Claude Code,
then say: **"Set this video up on YouTube."**

It reads your files, writes `squad/week/<date>-listing.md`, prints it, and stops. Then you
upload, set the thumbnail, paste the listing, pin the comment, and press publish, or set
the hour and let YouTube press it.

When it is live, come back and say: **"It is live: <your URL>."** That writes the row.

## What you get

One listing file you copy from at upload, and one row in `squad/content-log.md`: the
date, the title, the link, the video id. That row is the whole reason the Sunday read can
tell you which video brought the lead. A video with no row is invisible to it.

The booking link in the description and in the pinned comment carries
`?utm_source=youtube&utm_content=epNN`, your episode number. cal.com shows those two tags
on the booking's details page on its own, so a booking names the video that brought it
with nothing to set up.

## What it will not do

Upload the file. Schedule anything. Set your thumbnail. Write you a new title. Add a
second link to the description. Touch a spreadsheet or a calendar.
