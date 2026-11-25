# Google Calendar Bulk Delete

Bulk delete Google Calendar events by search term. Deletes ALL events whose title or description contains the entered text (not case sensitive).

![Demo](demo.gif)

## Usage

1. Open Google Calendar in **Month** view
2. Run script in browser console
3. Enter search text when prompted (e.g. `LSD` or `AppSyncId`)
4. Confirm deletion

## Features

- Searches event titles and descriptions
- Case-insensitive matching
- Processes up to 12 months
- Handles recurring events
- Progress tracking in console

## Title-only mode

Searching descriptions means opening every event that does not match by title, so it is slower on busy calendars. For a fast title-only search, set this at the top of `script.js`:

```js
const SEARCH_DESCRIPTION = false;
```

**Warning:** Permanent deletion. Cannot be undone. Try a narrow search term first.
