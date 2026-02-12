# README.md & Quick Start Guide

## Project Overview
This is a Universal AI Chat interface, a modern web-based chatbot supporting multiple AI providers like Anthropic (Claude models), OpenAI (GPT series), Google (Gemini), Meta (Llama), Mistral, Cohere, xAI (Grok), DeepSeek, and Perplexity. It features a sleek dark-themed UI with animated backgrounds, model selection, adjustable parameters (temperature, max tokens, top P), and real-time chat simulation. Currently in demo mode; production requires API key integration for live model responses. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)

## Key Features
- Multi-provider model selector with grouped options (e.g., Claude Opus 4.5, GPT-4o, Gemini 2.0 Flash). [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
- Customizable inference parameters via sliders: Temperature (0-2), Max Tokens (256-8192), Top P (0-1). [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
- Responsive design with sidebar (desktop) and mobile toggle, typing indicators, error handling. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
- JetBrains Mono and Crimson Pro fonts for a professional look; CSS variables for easy theming. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)

## Quick Start
1. Save `llm-chatbot.html` to your local machine or deploy to a static host like GitHub Pages or Vercel. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
2. Open `llm-chatbot.html` in any modern browser (Chrome, Firefox recommended). [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
3. Select a model from the sidebar dropdown (e.g., Claude Sonnet 4.5 as default). [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
4. Adjust parameters if needed (Temperature: 0.7, Max Tokens: 2048, Top P: 0.9). [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
5. Type a message in the input area and click "Send" (or Enter); view demo responses. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)

Demo shows simulated replies like "This is a demo interface... integrate the APIs". For mobile, tap the menu icon to open sidebar. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)

## Making It Production-Ready
Replace `simulateAPICall` function with real API fetches:
- Add API keys via environment variables or a config (e.g., `ANTHROPIC_API_KEY`).
- Use provider SDKs: Anthropic SDK for Claude, OpenAI SDK for GPT, etc.
- Update `sendMessage` to POST to endpoints like `https://api.anthropic.com/v1/messages`.
- Handle auth headers, streaming responses for typing effect.
Example stub in code: Integrate based on `state.currentModel` (e.g., if 'claude-sonnet-4', use Anthropic). [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)

## Tech Stack
- Pure HTML/CSS/JS (no frameworks needed). [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
- Google Fonts: JetBrains Mono, Crimson Pro. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
- CSS animations for grid background, message slides, typing dots. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)

## Customization
- Edit CSS variables in `:root` for colors (e.g., `--accent-primary: #00ffcc`). [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
- Add models by extending `<select>` options and `modelNames` object. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
- Extend parameters (e.g., add frequency penalty slider). [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)

## Troubleshooting
- Chat not responding? Ensure JS is enabled; check console for errors. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
- UI issues? Verify viewport meta tag for mobile. [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
- For real APIs, handle CORS if hosting locally (use `live-server` or similar). [ppl-ai-file-upload.s3.amazonaws](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/92098913/bb4bc56b-375d-4ad4-9c99-0e4d70b09cb6/llm-chatbot.html)
