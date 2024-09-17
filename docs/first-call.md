---
title: Making Your First TTS API Call
nav_order: 4
---

# Making Your First TTS API Call

Congratulations on obtaining your API key! This guide will walk you through making your first Text-to-Speech (TTS) API call with Dubverse, converting your text into natural-sounding speech.

## Prerequisites

Before you begin, ensure you have:

- Your Dubverse API key (If you haven't obtained one, visit the [API Key page](api-key.md))
- A tool for making HTTP requests (e.g., Postman, cURL, or your preferred programming language)

## API Request Details

### HTTP Method

```
POST
```

### Endpoint URL

```
https://macaque.dubverse.ai/api/merlin/services/tts/text-to-speech
```

### Headers

```
X-API-Key: YOUR_API_KEY_HERE
Content-Type: application/json
```

Replace `YOUR_API_KEY_HERE` with your actual Dubverse API key.

### Request Body

```json
{
  "text": "Hello, world! This is my first TTS API call.",
  "speaker": 181,
  "config": {
    "use_streaming_response": false
  },
  "callback_url": "https://your-callback-url.com/endpoint"
}
```

## Request Parameters Explained

- `text` (required): The input text you want to convert to speech.
- `speaker_no` (required): The ID of the speaker voice. See [Speaker Selection](speaker-selection.md) for available options.
- `config` (optional): Additional configuration options.
  - `use_streaming_response`: Set to `true` for streamed audio, `false` for a complete audio file response.
- `callback_url` (optional): URL to receive the API response if different from the origin.

## Making the API Call

You can use any HTTP client to make this API call. Here's an example using cURL:

```bash
curl -X POST "https://macaque.dubverse.ai/api/merlin/services/tts/text-to-speech" \
     -H "X-API-Key: YOUR_API_KEY_HERE" \
     -H "Content-Type: application/json" \
     -d '{
           "text": "Hello, world! This is my first TTS API call.",
           "speaker": 181,
           "config": {
             "use_streaming_response": false
           }
         }'
```

## Understanding the Response

### Success Response

For non-streamed responses:

- You'll receive a WAV file containing the synthesized speech.
- The response will have a `Content-Type: audio/wav` header.

For streamed responses:

- You'll receive audio data in chunks.
- The response will have a `Transfer-Encoding: chunked` header.

### Error Response

If an error occurs, you'll receive a JSON response with error details:

```json
{
  "error": {
    "code": "ERROR_CODE",
    "message": "Description of the error"
  }
}
```

## Next Steps

Now that you've made your first API call, you can:

1. Learn more about [Speaker Selection](speaker-selection.md)
2. Understand [Usage and Billing](usage-billing.md)

## Need Help?

If you encounter any issues during the account creation process:

- Contact our support team at friends@dubverse.ai

We're excited to see what you'll create with Dubverse TTS!

[← Back to Home](../index.md)
