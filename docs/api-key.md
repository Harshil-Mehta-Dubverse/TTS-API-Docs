# Obtaining Your API Key

An API key is required to authenticate your requests to our Text-to-Speech (TTS) API. Follow these steps to obtain your API key:

## Steps to Get Your API Key

1. Log in to your account on our main website [www.ourttssiteexample.com](https://www.ourttssiteexample.com).

2. Navigate to the TTS page. This is usually found in the main navigation menu or your account dashboard.

3. Look for a section labeled "API Keys" or "Create API Key".

4. Click on the "Generate New API Key" or similar button.

5. You may be asked to confirm this action or provide a name for your API key.

6. Your new API key will be displayed. Make sure to copy it and store it securely.

   **Important:** For security reasons, we may only show your API key once. If you lose it, you may need to generate a new one.

## Using Your API Key

To use the TTS API, you'll need to include your API key in the header of your API requests. The specific header to use is:

```
X-API-Key: your_api_key_here
```

Replace `your_api_key_here` with the actual API key you generated.

## API Key Security

- Keep your API key confidential. Don't share it publicly or commit it to version control systems.
- If you suspect your API key has been compromised, generate a new one immediately and update your applications.
- Consider using environment variables or secure key management systems in your applications to store the API key.

## Next Steps

Now that you have your API key, you're ready to [make your first API call](first-call.md).

If you have any issues generating or using your API key, please contact our support team for assistance.

[Back to Home](../index.md)