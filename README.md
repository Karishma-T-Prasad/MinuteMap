# MinuteMap — AI Meeting Workspace

MinuteMap is an AI-powered meeting workspace that converts rough meeting notes into structured, reviewable information. It helps users identify action items, decisions, deadlines, risks, unresolved questions, and missing information.

## Features

- **AI meeting analysis:** Extracts structured information from unorganized meeting notes.
- **Action item management:** Tracks tasks, owners, deadlines, and status.
- **Decision and risk identification:** Separates decisions, blockers, and unresolved questions.
- **Meeting history:** Keeps previously saved meeting records accessible.
- **Action overview:** Provides charts and summaries for tracking progress.
- **Email reminders:** Supports deadline-related notifications and reminder activity tracking.
- **User authentication:** Provides email-based sign-in and user-associated data.

## Technology Stack

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** JavaScript API endpoints
- **AI inference:** Cirrascale AI Suite, using the `Llama-3.1-8B` model in the current analysis endpoint
- **Database:** PostgreSQL
- **Email:** Gmail API integration with a platform-email fallback
- **Hosting:** Hatchable

## How It Works

1. The user enters rough meeting notes.
2. The backend sends the notes to the configured AI endpoint.
3. The AI returns labelled sections containing meeting information.
4. The application parses and displays the results for review.
5. The user saves the meeting and its action items.
6. The application stores records and supports task tracking.
7. A scheduled backend job checks eligible tasks and attempts to send reminders.

## Project Structure

- `public/` — Frontend pages, styling, and visual assets
- `api/` — AI analysis, meeting management, action items, and reminder endpoints
- `lib/` — Shared utilities, including email sending
- `migrations/` — Database table definitions and schema changes
- `hatchable.toml` — Hosting-specific configuration

## AI-Assisted Development

AI-assisted tools were used during development. The implementation is being reviewed and tested to understand its architecture, functionality, and design decisions. Individual contributions should be described accurately.

## Security Note

API keys, OAuth tokens, passwords, and private user data must not be committed to the public repository. Hosting secrets and integrations must be configured separately.

## Live Application

https://minutemap.hatchable.site
