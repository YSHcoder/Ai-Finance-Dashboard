# How to Set Up Gemini API for Receipt Scanning

The AI receipt scanning feature requires a valid Google Gemini API key. Follow these steps to get your own free API key:

## Steps to Get Gemini API Key:

1. **Visit Google AI Studio**
   - Go to: https://aistudio.google.com/app/apikey
   - Sign in with your Google account

2. **Create API Key**
   - Click "Get API Key" or "Create API Key"
   - Select "Create API key in new project" (or use existing project)
   - Copy the generated API key

3. **Add to Your Project**
   - Open `.env.local` file in your project
   - Replace the existing `GEMINI_API_KEY` value with your new key:
   ```
   GEMINI_API_KEY=your_new_api_key_here
   ```

4. **Restart the Development Server**
   - Stop the current server (Ctrl+C in terminal)
   - Run `npm run dev` again

## Free Tier Limits:

- 15 requests per minute
- 1,500 requests per day
- 1 million tokens per minute

This is more than enough for personal use and testing!

## Testing the Feature:

1. Go to "Add Transaction" page
2. Click "Scan Receipt with AI"
3. Upload a receipt image (JPG, PNG)
4. The AI will extract:
   - Amount
   - Date
   - Merchant name
   - Description
   - Suggested category

## Troubleshooting:

- **404 Error**: API key is invalid or model not available
- **Quota Error**: You've exceeded the free tier limits
- **Invalid Response**: The image might not be a clear receipt

If you don't want to use the AI feature, you can still manually enter transaction details!
