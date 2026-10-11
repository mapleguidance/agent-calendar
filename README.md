# Agent Work Calendar

Visible record of all agent work (Ulysses), kept as files in this repo so it
survives any single account or service.

- Events live in [`calendars/agent-work.yaml`](calendars/agent-work.yaml).
  Planned work is logged as future events; completed significant work is
  logged as past events with the outcome in the description.
- Every push rebuilds the `.ics` feed via GitHub Actions (see
  [`git-calendar`](https://github.com/coderefinery/git-calendar), the
  upstream template this repo was forked from) and publishes it to GitHub
  Pages.
- **Subscribe:** add the `.ics` URL to any calendar app (Google Calendar:
  Other calendars → From URL; Apple Calendar: File → New Calendar
  Subscription). The feed stays in sync automatically.
- Event text is sanitized for a public feed: no private details, no
  financial figures, no personal data.

To log work: edit `calendars/agent-work.yaml`, commit, push. The feed
rebuilds itself.
