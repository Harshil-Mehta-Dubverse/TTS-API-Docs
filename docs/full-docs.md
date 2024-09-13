# Full API Documentation

This page provides comprehensive documentation for our Text-to-Speech (TTS) API. Here you'll find detailed information about endpoints, request parameters, response formats, and more.

## Table of Contents

1. [Authentication](#authentication)
2. [API Endpoint](#api-endpoint)
3. [Request Parameters](#request-parameters)
4. [Response Formats](#response-formats)
5. [Error Handling](#error-handling)
6. [Rate Limits](#rate-limits)

## Authentication

All API requests must include your API key in the header:

```
X-API-Key: YOUR_API_KEY_HERE
```

Replace `YOUR_API_KEY_HERE` with your actual API key. If you haven't obtained an API key yet, please refer to the [API Key page](api-key.md).

## API Endpoint

The base URL for all API requests is:

```
https://api.ourttssiteexample.com/v1/tts
```

## Request Parameters

| Parameter | Type | Required | Description |
|-----------|------|----------|-------------|
| text | string | Yes | The text to convert to speech |
| speaker | integer | Yes | The ID of the speaker to use (see [Speaker Selection](speaker-selection.md)) |
| format | string | No | Audio format (default: "wav", options: "wav", "mp3", "ogg") |
| speed | float | No | Speech rate (0.5 to 2.0, default: 1.0) |
| pitch | float | No | Voice pitch (-20 to 20, default: 0) |
| stream | boolean | No | Whether to stream the audio (default: false) |

## Response Formats

### Non-streamed Response

For non-streamed requests, the API returns the audio file directly. The `Content-Type` header will match the requested format (e.g., `audio/wav` for WAV files).

### Streamed Response

For streamed requests, the API returns chunks of audio data with `Transfer-Encoding: chunked`. You'll need to handle the streaming on your end to reconstruct the audio.

## Error Handling

The API uses standard HTTP response codes. In case of an error, you'll receive a JSON response with more details:

```json
{
  "error": {
    "code": "ERROR_CODE",
    "message": "A description of the error"
  }
}
```

Common error codes include:
- 400: Bad Request
- 401: Unauthorized (invalid API key)
- 429: Too Many Requests (rate limit exceeded)
- 500: Internal Server Error

## Rate Limits

To ensure fair usage, we implement rate limiting:
- 100 requests per minute
- 1000 requests per hour
- 10000 requests per day

If you exceed these limits, you'll receive a 429 error. Please check the [Usage and Billing](usage-billing.md) page for more information on limits and how to increase them.

For any questions not covered here, please contact our support team.

[Back to Home](../index.md)