# Teacher Feedback

A mobile-first web app where students rate their teachers and write feedback about lessons. Only the school admin can read the reviews.

## Features

- **Find a teacher:** search by name or subject, filter by subject
- **Rate your experience:** score teaching quality, communication, clarity and student support from 1 to 5, or mark one "Not applicable"
- **Written feedback:** "What worked well?" and "What could be improved?", with an optional lesson or topic
- **Anonymous option:** students choose whether the admin sees their name
- **Language filter:** reviews with offensive words (English and Slovak) can't be sent
- **My reviews:** students see only their own reviews
- **Admin panel:** read all feedback, see averages per teacher, mark reviews as read, archive or delete them, manage teachers, set the term and school colour

## Who sees what

| | Own reviews | Other reviews | Scores |
|---|---|---|---|
| Student | ✅ | ❌ | ❌ |
| Teacher | — | ❌ | ❌ |
| Admin | ✅ | ✅ | ✅ |

## Run it

The whole app is one file, `index.html` (HTML, CSS and plain JavaScript, no build step).

- Open `index.html` in a browser, or
- In VS Code, install **Live Server**, right-click `index.html` and choose **Open with Live Server**.

The app comes with the LEAF Academy teachers built in. Run locally, it opens in **demo mode**: you can rate teachers and see the reviews in the Admin tab, but everything disappears when you reload the page.

## Status

Prototype. Saving data needs a database and school login (for example Firebase), which is the next step. All data access goes through one small `store` object in the code, so a database can be plugged in there.
