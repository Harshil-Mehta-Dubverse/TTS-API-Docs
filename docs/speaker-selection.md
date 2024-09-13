# Speaker Selection

Our TTS API offers a variety of speakers to choose from, allowing you to select the perfect voice for your application. This guide will help you understand how to select and use different speakers.

## Speaker Playground

To help you choose the right speaker, we provide a Speaker Playground on our main website. Here's how to use it:

1. Log in to your account at [www.ourttssiteexample.com](https://www.ourttssiteexample.com)
2. Navigate to the TTS page
3. Look for the "Speaker Playground" tab or section

In the Speaker Playground, you can:
- Select different languages
- Choose speaker genders
- Play sample audio for each available speaker
- See the associated speaker ID for use in API calls

## Using Speakers in API Calls

Once you've selected a speaker, you'll use its ID in your API calls. For example:

```json
{
  "text": "Hello, world!",
  "speaker": 12,
  "format": "wav"
}
```

In this example, `12` is the ID of the chosen speaker.

## Available Languages and Genders

We offer a wide range of languages and gender options. Some of our most popular include:

- English (US, UK, Australian)
- Spanish
- French
- German
- Mandarin Chinese
- Japanese

Each language typically has multiple gender options (e.g., male, female, neutral).

## Speaker Costs

All speakers are priced consistently based on the number of characters in the input text. For current pricing information, please check the [Usage and Billing](usage-billing.md) page.

## Best Practices

- Test multiple speakers for your use case to find the best fit
- Consider your target audience when selecting a speaker (e.g., region-specific accents)
- Remember that speaker IDs may change over time, so always refer to the Speaker Playground for the most up-to-date IDs

For any questions about speaker selection or if you need a specific type of voice not currently offered, please contact our support team.

[Back to Home](../index.md)