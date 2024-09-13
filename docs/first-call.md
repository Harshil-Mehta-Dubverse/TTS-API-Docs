# Making Your First API Call

Now that you have your API key, let's make your first call to our Text-to-Speech (TTS) API. This guide will walk you through a basic example to convert text to speech.

## Prerequisites

- Your API key (obtained from the [API Key page](api-key.md))
- A tool to make HTTP requests (e.g., cURL, Postman, or your preferred programming language)

## Basic API Call

Here's a simple example using cURL:

```bash
curl -X POST "https://api.ourttssiteexample.com/v1/tts" \
     -H "X-API-Key: YOUR_API_KEY_HERE" \
     -H "Content-Type: application/json" \
     -d '{
           "text": "Hello, world! This is my first TTS API call.",
           "speaker": 1,
           "format": "wav"
         }'
```

Replace `YOUR_API_KEY_HERE` with your actual API key.

## Request Parameters

- `text`: The text you want to convert to speech (required)
- `speaker`: The ID of the speaker voice you want to use (required, see [Speaker Selection](speaker-selection.md))
- `format`: The desired audio format (optional, defaults to "wav")

## Response

If successful, you'll receive a response with the audio data. For non-streamed responses, you'll get a WAV file. For streamed responses, you'll receive the audio data in chunks.

## Next Steps

- Explore more [API options and parameters](full-docs.md)
- Learn about [speaker selection](speaker-selection.md)
- Understand [usage limits and billing](usage-billing.md)

If you encounter any issues, please check our [full documentation](full-docs.md) or contact our support team.

[Back to Home](../index.md)