# Project Plan -- Multi-POV Compilation Platform

## Working Vision

Build a backend-first platform that automates creating synchronized
multi-POV videos from livestream VODs.

## Guiding Principles

-   Solve one core problem first.
-   Backend before frontend.
-   API-first architecture.
-   Every new feature should solve a real problem.

## Suggested Tech Stack

-   Python 3.12+
-   FastAPI
-   PostgreSQL (SQLite during early development is fine)
-   SQLAlchemy + Alembic
-   FFmpeg
-   yt-dlp
-   Docker
-   GitHub Actions
-   Pytest

------------------------------------------------------------------------

# Phase 0 -- Technical Proof of Concept

Goal: Produce a synchronized MP4 from a few manually supplied VOD URLs.

Deliverables: - Download video - Trim by timestamp - Synchronize clips -
Export one final video

Success: One command creates a correct compilation.

------------------------------------------------------------------------

# Phase 1 -- Retrieval Engine

Goals: - Download VODs - Cache downloads - Resume interrupted
downloads - Support partial downloads where possible

------------------------------------------------------------------------

# Phase 2 -- Data Layer

Entities: - Streamer - Stream - Event - Group (gta RP) - Bookmark - Clip

Features: - Store VOD metadata - Search by UTC - Relate streamers to
events

------------------------------------------------------------------------

# Phase 3 -- Timeline Engine

Create an internal timeline model.

Support: 
- POV switches
- Split-screen
- Transitions
- Export to MP4

Future:
- Export Premiere/Resolve timelines.

------------------------------------------------------------------------

# Phase 4 -- REST API

Endpoints: 
- Events
- Streams
- Bookmarks
- Jobs
- Processing
- Uploads

------------------------------------------------------------------------

# Phase 5 -- Web UI

Views: - Dashboard - Timeline - Stream selector - Processing queue -
Settings


------------------------------------------------------------------------

# Phase 6 -- Automation

-   Background workers
-   Progress tracking
-   Notifications
-   Retry failed jobs

------------------------------------------------------------------------

# Phase 7 -- AI Features

Possible ideas: - Highlight detection - Speaker detection - OCR -
Automatic POV suggestions - Title generation - Thumbnail generation


------------------------------------------------------------------------

# Phase 8 -- Publishing

-   YouTube upload
-   Metadata templates
-   Scheduling
-   Playlist support

------------------------------------------------------------------------

# Long-Term Goals

-   Plugin system
-   Desktop client
-   Public API
-   Multiple streaming platforms
-   Team collaboration

------------------------------------------------------------------------

# Definition of Success

The project should: - Be useful to real creators.
- Demonstrate backend engineering skills.
- Have automated tests.
- Be Docker deployable.
- Be documented well.
- Be something you actively use.
