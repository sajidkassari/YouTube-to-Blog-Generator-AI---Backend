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
   git clone https://github.com/sajidkassari/YouTube-to-Blog-Generator-AI---Backend.git
   
2. **Install Dependencies**

   ```bash
   cd YouTube-to-Blog-Generator-AI---Backend
   pip install -r requirements.txt
   
3. **Set Up Environment Variables**

Create a .env file in the root directory and add your environment variables:

   ```bash
   GEMINI_API_KEY=your_gemini_api_key
```
4. **Initialize the Database**
Run the following command to set up the SQLite database:

   ```bash
   python init_db.py
   
5. **Run the Application**

   ```bash
   python app.py
   
The backend will run on http://localhost:5000 by default.

**Deployment**
The backend is deployed on Vercel. You can access the live API at Vercel URL.

API Endpoints
POST /generate_blog: Generates a blog post from a YouTube video URL.
