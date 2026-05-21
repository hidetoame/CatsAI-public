# Google OAuth Verification Notes

CatsAI uses Google Calendar OAuth only when the user enables the schedule feature.

Requested scopes:

- `https://www.googleapis.com/auth/calendar.readonly`
- `https://www.googleapis.com/auth/calendar.events`

Scope justification:

- `calendar.readonly`: used to check the user's upcoming calendar events when the user asks CatsAI to confirm their schedule.
- `calendar.events`: used to add a calendar event when the user asks CatsAI to create a schedule.

CatsAI does not use Google Calendar data for advertising, analytics resale, or unrelated purposes.
