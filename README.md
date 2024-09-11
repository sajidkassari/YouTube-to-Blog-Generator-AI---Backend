# YouTube to Blog Generator AI - Backend

This is the backend part of the YouTube to Blog Generator AI project. It provides an API for converting YouTube video subtitles into SEO-friendly blog posts.

## Features

- Accepts YouTube video URLs
- Fetches subtitles using YouTube Transcript API
- Generates blog posts with Google Gemini API
- Limits to 5 conversions per unique IP per day

## Technologies Used

- Flask
- SQLite for IP tracking and conversion limits
- Google Gemini API
- YouTube Transcript API
- Vercel for deployment

## Setup

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/backend-repo.git
