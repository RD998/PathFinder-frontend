# Vital Path

A patient navigation platform that helps users find accessible, language-matched healthcare facilities, book appointments, manage a waitlist, and track required documents before a visit.

Built for PS3: The Missing Link — Patient Journey & Healthcare Access Navigator (Team Route 200).

## Structure

This is a two-part project:

| Part | Stack | Details |
|---|---|---|
| **Backend** | FastAPI + SQLAlchemy + PostgreSQL | See [README.md](README.md) |
| **Frontend** | Vanilla HTML/CSS/JS | See [README_frontend.md](README_frontend.md) |

## Deployment

| Part | Where |
|---|---|
| Backend API | [Render](https://pathfinder-backend-2u7u.onrender.com) |
| Database | Neon (PostgreSQL) |
| Frontend | GitHub Pages *(add the live URL here)* |

## Core Features

- Facility discovery filtered by accessibility needs and language
- Department → doctor → time slot booking funnel
- Reschedule and cancel appointments
- Waitlist: cancelling a slot automatically hands it to the next waiting patient
- Document prep checklist (government ID, prior prescription, referral letter)

## Notes

- Auth is intentionally minimal for this hackathon scope: login returns a `user_id` that the frontend carries on subsequent requests, no token/session system.
- Render's free tier and Neon's free tier both spin down when idle — the first request after inactivity can take a few seconds to respond.
