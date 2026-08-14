# Invitation Message Generator

A browser-based tool that merges a contact roster into personalized WhatsApp
invitations — one click per recipient, with message formatting preserved and
send status tracked.

**[Live demo →](https://felixgunawan25.github.io/invitation-message-generator/)**

> All names and phone numbers in this demo are placeholders. The original
> roster contains personal contact data and is not included in this repository.

## The problem

Sending a formal invitation to 17 alumni meant rewriting the same message 17
times, changing the name and honorific each time. Manual editing at that scale
is slow and error-prone — and WhatsApp silently collapses paragraph spacing
when text is pasted from most sources.

## What it does

- Merges roster fields (`name`, `cohort`, `honorific`, `time of day`) into a
  message template
- Preserves blank lines exactly, so the message pastes into WhatsApp intact
- Per-recipient copy button, with an override dropdown for the honorific
- Live preview and a template view showing the merge fields
- Tracks which recipients have been contacted
- Flags data issues automatically: duplicate numbers, missing numbers, and
  entries needing manual verification

## Notes

Runs entirely in the browser — no data leaves the page, no server involved.
Sending stays manual: the tool prepares and tracks messages, it does not
auto-send.

## Built with

HTML, CSS, vanilla JavaScript. No dependencies.
