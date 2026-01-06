# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a humorous web application that "fixes" a poorly-written JavaScript recruiting email. The project is intentionally simple and has **no build system, no tests, and no dependencies** beyond Bootstrap loaded via CDN.

See [README.md](README.md) for the full story and context.

## Architecture

**Single-page application with three files:**
- [index.html](index.html) - Static HTML page with Bootstrap UI
- [recruiter-email.js](recruiter-email.js) - Constructor function that manages state and UI interactions
- [README.md](README.md) - Humorous code review of the original recruiter email

**Key architectural notes:**
- `RecruiterEmail` is a constructor function (not a class) that creates an interactive recruiting pitch presentation
- State is managed through closure variables (`currentPitch`, `elements`, `pitches`, `affirmativeResponses`)
- The constructor takes two parameters: `recipient` (string) and `sender` (object with firstName, lastName, phone, email)
- DOM manipulation is vanilla JavaScript (no framework)
- The user cycles through pitches by clicking affirmative responses; after the final pitch, clicking triggers a `mailto:` link

## Development

**No build process.** Simply open [index.html](index.html) in a browser to run the application.

**Deployment:** This is deployed to GitHub Pages at https://riebschlager.github.io/linkedin-recruiter-email/

## Code Style Notes

- Uses ES6 features (let, const, template literals, arrow functions)
- Intentionally minimal - the humor is in the simplicity vs. the original email's complexity
- Constructor pattern with public methods exposed via `this`
