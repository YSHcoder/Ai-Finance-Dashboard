# How to Fix Gemini API - Complete Guide

## The Problem
Your API keys are not working because the **Generative Language API** is not enabled in your Google Cloud project.

## Complete Solution (Step by Step)

### Step 1: Go to Google AI Studio
1. Visit: https://aistudio.google.com/
2. Sign in with your Google account

### Step 2: Enable the API
1. Click on "Get API Key" in the left sidebar
2. You'll see a message about enabling the API
3. Click "Enable API" or "Enable Generative Language API"
4. Wait for it to be enabled (may take a few seconds)

### Step 3: Create API Key
1. After the API is enabled, click "Create API Key"
2. Choose "Create API key in new project" (recommended)
3. Copy the generated API key

### Step 4: Verify the API Key Works
1. Go to: https://aistudio.google.com/app/prompts/new_chat
2. Try typing a message - if it works, your API is enabled!

### Step 5: Update Your Project
Replace the `GEMINI_API_KEY` in your `.env.local` file with the new key.

## Alternative: Enable API via Google Cloud Console

If the above doesn't work:

1. Go to: https://console.cloud.google.com/
2. Select your project (or create a new one)
3. Go to "APIs & Services" > "Library"
4. Search for "Generative Language API"
5. Click on it and press "Enable"
6. Go to "APIs & Services" > "Credentials"
7. Create a new API key
8. Copy and use this key

## Testing Your API Key

After getting a new key, you can test it here:
https://aistudio.google.com/app/prompts/new_chat

If you can chat with Gemini there, your API key will work in the app!

## Current Status

The AI scan feature is currently not working because:
- The API key doesn't have access to Gemini models
- The Generative Language API is not enabled

You can still use the app by manually entering transaction details!
