# Meeting Minutes Generator

An AI-powered tool that transcribes audio meetings, generates structured meeting minutes, and creates email drafts.

## Technologies Used

- **CrewAI**: Orchestrates AI agents for meeting minutes generation
- **OpenAI Whisper**: Audio transcription
- **Google Gmail API**: Email draft creation
- **Pydub**: Audio file processing
- **Python**: Core programming language

## Features

- Audio transcription from WAV files
- Structured meeting minutes generation
- Action items extraction
- Sentiment analysis
- Automatic email draft creation

## Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up environment variables in `.env`:
   ```
   OPENAI_API_KEY=your_key
   AGENTOPS_API_KEY=your_key
   GMAIL_SENDER=your_email
   GMAIL_RECIPIENT=recipient_email
   ```
4. Place your audio file (WAV format) in the project directory

## Usage

Run the main script:
```bash
python src/meeting_minutes/main.py
```

## Output

Generated files will be saved in the `meeting_minutes_text` directory:
- `summary.txt`: Meeting summary
- `action_items.txt`: Extracted action items
- `sentiment.txt`: Meeting sentiment analysis
- The email draft will be in your gmail and assigned to be sent to the email and have set in the .env file
