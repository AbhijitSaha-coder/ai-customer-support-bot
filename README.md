# AI Customer Support Chatbot

An AI-powered chatbot that answers customer questions automatically using a business's own information — hours, pricing, services, location.

**Demo:** [https://youtu.be/V5uRP8jX6-g](https://youtu.be/V5uRP8jX6-g)

## How it works

- Built with n8n for automation/orchestration
- Uses Google Gemini API for natural language understanding
- Deployed via Telegram (also adaptable to WhatsApp or a website widget)
- Answers only from the business's actual provided information — declines gracefully rather than guessing when it doesn't know something

## Example

- "What are your hours?" → accurate reply pulled from business data
- "Do you accept insurance?" → correctly declines to guess, redirects to calling the business

## Setup

1. Import `workflow.json` into your n8n instance
2. Add your own Telegram bot credentials (via [@BotFather](https://t.me/BotFather))
3. Replace `YOUR_GEMINI_API_KEY_HERE` in the HTTP Request node's URL with your own [Gemini API key](https://aistudio.google.com)
4. Update the `business_info` field in the Edit Fields node with your actual business details
5. Activate the workflow

Built by Abhijit Saha — available for custom builds for your business.
