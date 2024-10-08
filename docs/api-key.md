---
title: Obtaining Your API Key
nav_order: 3
---

# Obtaining Your API Key

Welcome to the API key generation process! Your API key is the gateway to accessing Dubverse's powerful Text-to-Speech (TTS) capabilities. This guide will walk you through obtaining and securing your API key.

## Generating Your API Key

Follow these steps to create your Dubverse API key:

1. **Access Your Dubverse Account**

   - Visit [https://webapp.dubverse.ai/](https://webapp.dubverse.ai/){:target="\_blank"}
   - Log in with your credentials

2. **Navigate to the TTS API Section**

   - Look for "TTS API" in the main navigation menu
   - Click to access the TTS API dashboard

3. **Locate the API Key Management Area**

   - Find the section labeled "API Key"

4. **Generate Your New API Key**

   - Click the "Create Key" button
   - A new API key will be generated instantly

5. **Secure Your API Key**

   - Copy the displayed API key immediately
   - Store it in a secure location (we recommend using a password manager)

## Implementing Your API Key

To authenticate your requests to the Dubverse TTS API, include your API key in the header of each request:

```
X-API-Key: your_api_key_here
```

Replace `your_api_key_here` with your actual API key.

## Best Practices for API Key Security

Protecting your API key is crucial. Follow these best practices:

1. **Keep It Confidential**

   - Never share your API key publicly
   - Avoid committing it to version control systems

2. **Use Environment Variables**

   - Store your API key as an environment variable in your development and production environments

3. **Implement Key Rotation**

   - Regularly generate new API keys and update your applications

4. **Monitor Usage**

   - Regularly check your API usage logs for any suspicious activity

5. **Revoke Compromised Keys**
   - If you suspect your key has been compromised, revoke it immediately and generate a new one

## What's Next?

Now that you have your API key, you're ready to harness the power of Dubverse TTS:

1. [Make Your First API Call](first-call.md) - Start converting text to speech

## Need Help?

If you encounter any issues during the account creation process:

- Contact our support team at friends@dubverse.ai

We're excited to see what you'll create with Dubverse TTS!

[← Back to Home](../index.md)
