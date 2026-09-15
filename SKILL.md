---
name: publish
description: Use this when the cut is finished and the video needs its YouTube listing. The founder says "set this video up on YouTube", "write the listing", "do the description and the chapters", "/publish", and later "here is the link", "it is live" or "the video is up" with the URL. It writes the listing the founder pastes into YouTube Studio, the announcement post that goes out the same hour, and one row in squad/content-log.md. It never touches YouTube and it never sends the announcement.
---

# Publish

Turn the finished cut into a listing the founder pastes into YouTube Studio, then log the
one row that makes the video countable.

**You never touch YouTube.** No upload, no schedule, no thumbnail, no tag typed into an
account, no end screen set for them. You write the announcement post; the founder's own
line sends it. There is no connector in this run and you never ask for one.

Say this line once, in your first message on a fresh run: This skill is a base. Once you
have done it your way, tell your squad "update the skill to do it like this."

`.claude/squad-roots.md` is the per-repo instance file every member-run skill reads first
(founder name, product word, the `week`, `episodes` and `content log` paths), and its
values win over the `squad/` paths below, which are worked examples. `<date>` is the date
the package file carries.

**Resuming, off the outputs on disk.** No `squad/week/<date>-listing.md`: start at the
sources. The listing is there and the video is not live: print it and the by-hand list
again. A URL and no row with that video id in `squad/content-log.md`: write the row
and the announcement. A row with that id and an `## ANNOUNCEMENT` block already there: done.

## The outputs

1. `squad/week/<date>-listing.md`: the title, the description, the chapters and the pinned
   comment, and nothing the founder does not paste. The booking link in the description and in the
   pinned comment carries `?utm_source=youtube&utm_content=epNN`, so every booking names
   the episode that brought it. The `## ANNOUNCEMENT` block joins this file once the video
   is live.
2. `squad/content-log.md`: ONE row appended per video, columns
   `date | title | link | video id`. c5 reads every row on Sunday.
3. `.claude/squad-roots.md`: the `content log` row when it carries none. Nothing else in
   it touched.

## The sources

| What | Where | What it gives |
|---|---|---|
| the package | `squad/week/<date>-package.md`, the latest (or `<date>-repackage.md` when this video was repackaged) | the MAIN title, the TEST line, and `episode:` naming the episode folder, `epNN`, which is also the tag the booking link carries |
| the finished cut | `06_CAPTIONS.srt`, the caption file the cut wrote | the real timings the chapters come from |
| the script | `03_SCRIPT.md` in that episode folder | the hook line and the tools named on camera |
| the sales script | `squad/sales.md` | the booking link, which is the one call to action |

**No package file, or a package with no locked title: STOP on one line.** The title is
`the-proven-package`'s and this run never makes one up.

**No `06_CAPTIONS.srt` in the episode folder: ask for it and stop.** Never guess a
timestamp, and never take chapters off the script.

**No `squad/sales.md`: STOP on one line.** The booking link is g6's, and a listing with no
link is a video that cannot make money. Say to run g6 and come back; write nothing.

## The title

Copy the MAIN title out of the package, character for character. **Never re-title.** A
founder who wants a different title wants `the-proven-package`.

## The description

This order, no improvising:

1. **ONE call to action at the top**, as `Phrase : URL`. The booking link from
   `squad/sales.md` with `?utm_source=youtube&utm_content=epNN` on the end, NN the episode
   number off the package's `episode:` line (ep01 stays ep01). A link that already carries
   a `?` gets the 2 tags joined on with `&` instead.
2. A hook line.
3. One plain paragraph for search, in the words a buyer would type.
4. The `CHAPTERS` block.
5. `THE STACK`: the tools named in the video, each a plain link.

One call to action, so one opt-in link. 2 links maximum: the booking link, and the one
tool in THE STACK the video actually runs on.

Plain URLs only. No redirect through another site, no shortener. No em dashes anywhere;
this is outward-facing.

## The listing, then stop

**Chapters, off the finished cut.** First chapter at `0:00` or YouTube throws out the
whole list. 3 minimum, each at least 10 seconds, named for what is on screen at that
timestamp.

**No tags, no end screen.** The file holds exactly what the founder pastes into Studio.

**The pinned comment, as text.** The call to action line again, the phrase and the same
tagged booking link, for the founder to post first and pin.

Write `squad/week/<date>-listing.md` with all of it and print it. The founder reads it
once and fixes a word.

Then stop, and say what is left, all of it by hand in YouTube Studio:

- Upload the file, add `06_CAPTIONS.srt` as the subtitle track.
- Set the thumbnail from the package's main pair, paste the listing, post the pinned
  comment and pin it.
- Add all 3 pairs in Test & Compare, title and thumbnail together.
- Set the hour and let YouTube press it.

Never upload or schedule the video yourself, and never offer to.

## The announcement

The founder hands over the video's URL, which YouTube Studio gives them the moment the video is
scheduled, so this is written then and not before. Append an `## ANNOUNCEMENT` block to
`squad/week/<date>-listing.md`:

    ## ANNOUNCEMENT
    Networks: Threads, Facebook
    Image: squad/week/thumbs/<date>/<the main pair's 1280x720 file>
    Post:
    <3 or 4 lines, then the video URL on its own last line>

ONE version of the text, never a variant per network. The lines are the hook line off `03_SCRIPT.md` and what the video shows, in the
founder's own words off the script. No hashtags. **The only link is the plain video URL**, never
the tagged booking link: the description carries that, and a second ask here splits the count.

Then say where it goes, and stop: the founder pastes it themselves, in the hour the video
goes live, on the platform they already post on. Never offer to send it and never ask for a
connector.

## The row

The founder handed over the URL. Append ONE row to `squad/content-log.md`:
`date | title | link | video id`. Today's date, the locked title, the URL, and the id
after `v=`. Create the file with that header row when it does not exist, and add the
`content log` row to `.claude/squad-roots.md` when it carries none. Never a second row for
a video id already in the file.

## Rules

- **Never touch YouTube.** No upload, no schedule, no thumbnail, no tag typed into any
  account. The announcement is written here and sent by the founder's own line.
- **Never write a title.** The package locked it.
- **Never invent a timestamp.** Chapters come off the finished cut or the run stops.
- **Never a second call to action.**
- **Never price past what `squad/business.md` carries.**
- **Never invent a number, a name or a need**, and never put a number, a claim or a tool
  in the description that the video does not carry. Never paraphrase a line of the script
  into something the founder did not say.
- **Never write to a spreadsheet, a calendar or an account.** This run touches 2 files in
  `squad/` and one roots row.
- **Never send the announcement.** It is written here and pasted by the founder's own hand.
