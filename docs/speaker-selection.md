---
title: Speaker Selection
nav_order: 5
---

# Speaker Selection

Choosing the right voice for your Text-to-Speech (TTS) application is crucial for creating an engaging user experience. Dubverse offers a diverse range of high-quality voices across multiple languages and accents. This guide will help you navigate our speaker options and select the perfect voice for your project.

## Exploring the Speaker Playground

Our Speaker Playground is a powerful tool designed to help you audition and select the ideal voice for your TTS needs.

### Accessing the Speaker Playground

1. Log in to your Dubverse account at [https://webapp.dubverse.ai/](https://webapp.dubverse.ai/){:target="\_blank"}
2. Navigate to the "TTS API" page in the main menu
3. Click on the "Speakers" tab

### Features of the Speaker Playground

- **Language Filtering**: Easily filter voices by language or dialect
- **Gender Selection**: Choose between male, female, and neutral voice options
- **Audio Sampling**: Listen to high-quality audio samples for each voice
- **Speaker Details**: View comprehensive information about each voice, including:
  - Speaker Number (for API calls)
  - Language

## Implementing Speakers in Your API Calls

Once you've chosen a speaker, use its Number in your API requests:

```json
{
  "text": "Welcome to Dubverse TTS! How can I assist you today?",
  "speaker_no": 181
}
```

In this example, `181` represents the chosen speaker's Number.

## Best Practices for Speaker Selection

1. **Know Your Audience**: Choose a voice that resonates with your target demographic in terms of language, accent, and style.

2. **Consider Context**: Select a voice appropriate for your application's purpose (e.g., a professional tone for business applications, a friendly voice for customer service bots).

3. **Test Thoroughly**: Use the Speaker Playground to test your specific content with multiple voices before making a final decision.

4. **Consistency is Key**: Stick to one voice per character or purpose in your application to maintain a coherent user experience.

5. **Stay Updated**: Regularly check the Speaker Playground for new voices that might better suit your needs.

6. **Localization**: For global applications, consider using region-specific accents to enhance user engagement and authenticity.

## Speaker Costs and Billing

Dubverse maintains a consistent pricing model across all speakers, based on the number of characters processed. This approach ensures fairness and predictability in your TTS costs.

For detailed pricing information and to understand how billing works, please refer to our [Usage and Billing](usage-billing.md) page.

## Customization and Special Requests

Need a specific voice or accent not currently available in our library? We're here to help!

- **Language Expansion**: Request support for additional languages or dialects.

Contact our support team at friends@dubverse.ai to discuss your specific requirements.

## Need Assistance?

If you have any questions about speaker selection or need guidance in choosing the right voice for your project:

- Reach out to our support team at friends@dubverse.ai

We're excited to help you find the perfect voice for your TTS application!

[← Back to Home](../index.md)
