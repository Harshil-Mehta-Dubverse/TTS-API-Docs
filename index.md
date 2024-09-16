---
title: Welcome to Our TTS API Documentation
nav_order: 1
---

# Welcome to Our Text-to-Speech (TTS) API Documentation

Welcome to the Dubverse TTS API documentation. This guide provides quick reference for experienced users and comprehensive information for new integrators.

## API Quick Reference

### Endpoint

```
POST https://macaque.dubverse.ai/api/merlin/services/tts/text-to-speech
```

### Headers

```
X-API-Key: YOUR_API_KEY_HERE
Content-Type: application/json
```

### Request Body

```json
{
  "text": "Hello, welcome to Dubverse TTS!",
  "speaker": 181,
  "config": {
    "use_streaming_response": false
  }
}
```

### Sample cURL Request

```bash
curl -X POST "https://macaque.dubverse.ai/api/merlin/services/tts/text-to-speech" \
     -H "X-API-Key: YOUR_API_KEY_HERE" \
     -H "Content-Type: application/json" \
     -d '{
           "text": "Hello, welcome to Dubverse TTS!",
           "speaker": 181,
           "config": {
             "use_streaming_response": false
           }
         }'
```

## Key Features

- High-quality text-to-speech conversion
- Multiple speaker options
- Customizable speech parameters
- Streamed and non-streamed audio output

## Quick Start Guide

1. [Create Your Account](docs/account-creation.md)
2. [Obtain Your API Key](docs/api-key.md)
3. [Make Your First API Call](docs/first-call.md)

## Documentation Sections

- [Speaker Selection Guide](docs/speaker-selection.md)
- [Usage and Billing](docs/usage-billing.md)

## Getting Help

If you need assistance or have any questions, please don't hesitate to contact our support team.

Thank you for choosing our TTS API. We're excited to see what you'll create!
