# Clypto — AI-Powered Video Repurposing

**Discover engaging video moments. Analyze transcripts with AI. Create short-form content.**

Clypto is a local AI-powered video repurposing application designed to help content creators identify interesting moments in YouTube videos and transform selected segments into short-form content.

It combines trend discovery, AI-assisted clip analysis, automated video processing, and customizable short-form editing workflows in one interface.

> **Project status:** Local application / prototype. Not currently deployed as a public web service.

## Overview

Clypto aims to simplify the video repurposing workflow:

1. Discover trending topics.
2. Find relevant YouTube videos or paste a video URL.
3. Retrieve video transcripts and identify potential highlights using AI.
4. Select and create video clips.
5. Transform clips into vertical short-form formats.
6. Customize captions, hooks, branding, and other editing options.
7. Process multiple selected clips through batch workflows.

## Key Features

- **Trend Discovery:** Aggregates topic signals from Google Trends, Reddit, and GDELT news sources.
- **YouTube Discovery:** Search videos by topic, upload period, and minimum view count.
- **AI Clip Analysis:** Uses transcript-based analysis to suggest potential clips with timestamps, titles, opening words, and hook-strength scores.
- **Video Transcription:** Supports YouTube captions and local speech-to-text processing through Faster-Whisper.
- **Automated Clipping:** Uses yt-dlp and FFmpeg to download and extract selected video segments.
- **Short-Form Transformation:** Supports vertical 9:16 output, subtitle styles, hook overlays, and export profiles.
- **Batch Processing:** Processes multiple selected clips through a sequential job queue.
- **Channel Branding:** Supports watermarks, banners, intro/outro assets, and configurable editing defaults.
- **Progress Tracking:** Reports download and video-processing progress.

## Technology Stack

| Area | Technologies |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | Python, FastAPI |
| AI Integration | OpenAI API, Anthropic API |
| Transcription | YouTube Transcript API, Faster-Whisper |
| Video Processing | FFmpeg, yt-dlp, PyAV |
| Computer Vision | OpenCV, Pillow |
| Trend Research | Google Trends, Reddit API, GDELT |
| Data Storage | SQLite |
| Data Processing | NumPy, RapidFuzz |

## High-Level Architecture

```text
                 CLYPTO
                   |
          Frontend Interface
           HTML / CSS / JS
                   |
                FastAPI
                   |
       +-----------+-----------+
       |           |           |
   AI Analysis  Discovery   Media Pipeline
       |           |           |
   OpenAI       Google       yt-dlp
   Anthropic    Reddit       FFmpeg
                GDELT        OpenCV
       |           |           |
       +-----------+-----------+
                   |
          Local Storage
          SQLite / Outputs
```

## Project Focus

Clypto explores practical applications of:

- AI-assisted content analysis
- Python backend development
- API integration and orchestration
- Automated video processing
- Speech-to-text workflows
- Computer vision
- Background job processing
- Local application architecture

## Current Development Status

Clypto is being developed and tested as a local application.

The public repository is a project showcase. Proprietary application source code, private configuration, credentials, and API keys are not included.

Some features depend on external APIs, configured credentials, and local media-processing resources.

## Security and Privacy

- AI provider keys are designed to be stored outside the project directory.
- Private credentials and environment configuration are excluded from this showcase.
- The current application is designed around a local, single-user workflow and should not be exposed as a public service without additional security and deployment work.

## Project Showcase

This repository documents the concept, architecture, technologies, and development direction of Clypto.

Screenshots and demonstration media can be added as the interface and workflows are prepared for public presentation.

---

**Clypto — Turning long-form video into short-form opportunities.**
