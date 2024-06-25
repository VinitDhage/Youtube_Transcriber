# Youtube_Transcriber

This is a Streamlit application that extracts transcripts from YouTube videos and summarizes them using Google Gemini Pro's generative AI model. The application provides detailed notes in a concise format, making it easier to understand the key points from the video.

## Features

- Extracts transcripts from YouTube videos using the `youtube_transcript_api`.
- Generates summaries of transcripts using Google Gemini Pro.
- Displays a thumbnail of the YouTube video.
- Provides detailed notes in a readable format.

## Requirements

- Python 3.7 or higher
- Streamlit
- python-dotenv
- youtube_transcript_api
- google-generativeai

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/VinitDhage/yt-transcript-notes-converter.git
    cd yt-transcript-notes-converter
    ```

2. Create and activate a virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Create a `.env` file in the root directory of the project and add your Google API key:

    ```text
    GOOGLE_API_KEY=your_google_api_key_here
    ```

## Usage

1. Run the Streamlit app:

    ```bash
    streamlit run app.py
    ```

2. Open the provided URL in your web browser.

3. Enter a YouTube video link in the input field.

4. Click on "Get Detailed Notes" to generate and display the summarized notes.

## Project Structure

- `app.py`: The main application script.
- `requirements.txt`: A file containing all the required Python packages.
- `.env`: A file to store environment variables, such as the Google API key.

## How It Works

1. The application takes a YouTube video link as input.
2. It extracts the video ID from the link.
3. The YouTube Transcript API fetches the transcript of the video using the video ID.
4. The transcript is combined into a single string.
5. The combined transcript is sent to Google Gemini Pro's generative AI model along with a summarizing prompt.
6. The AI model generates a summary, which is then displayed in the application.


## Acknowledgments

- [Streamlit](https://streamlit.io/)
- [python-dotenv](https://github.com/theskumar/python-dotenv)
- [YouTube Transcript API](https://github.com/jdepoix/youtube-transcript-api)
- [Google Generative AI](https://developers.google.com/generative-ai)


