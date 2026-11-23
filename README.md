# Jannat AI

WhatsApp-style Jannat AI chat using a secure Vercel serverless function and Gemini API. The Gemini key is never placed in `index.html`.

## Vercel setup

In the Vercel project settings, open **Environment Variables** and add:

- Name: `GEMINI_API_KEY`
- Value: your Gemini API key
- Environments: Production, Preview, and Development

Optional model variable: `GEMINI_MODEL=gemini-3.5-flash-lite`.
After saving the variable, redeploy the project. The frontend calls `/api/chat` and the serverless function calls Gemini.
