# AI Trend Bot

Posts daily creative/sarcastic updates of trending topics from Mastodon ("X") using OpenAI.

## Setup

1. Clone this repo.  
2. `cd ai-trend-bot`  
3. `./scripts/setup_env.sh`  
4. Fill in your `.env` from `.env.example`.  
5. `./scripts/run_bot.sh` to fetch, generate, and post.

## Folder Layout

\`\`\`
ai-trend-bot/
├── data/
│   └── raw/            # (optional) cache raw API dumps
├── src/
│   └── ai_trend_bot/
│       ├── __init__.py
│       ├── config.py
│       ├── mastodon_client.py
│       ├── trend_fetch.py
│       ├── post_generator.py
│       └── pipeline.py
├── scripts/
│   ├── setup_env.sh
│   └── run_bot.sh
├── tests/
│   ├── test_trend_fetch.py
│   └── test_post_generator.py
├── .env.example
├── requirements.txt
└── README.md
\`\`\`

## Testing

\`\`\`bash
pytest
\`\`\`
