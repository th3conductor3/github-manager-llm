# GitHub Manager for LLMs

A web interface that allows any LLM to manage GitHub repositories through a simple API.

## Features

- List all repositories
- Create new repositories
- Delete repositories
- Clean web interface
- REST API for programmatic access

## Deploy to Vercel

1. Fork this repository
2. Go to [vercel.com](https://vercel.com) and sign in with GitHub
3. Import this repository
4. Add environment variable:
   - `GITHUB_TOKEN` = your GitHub personal access token
5. Deploy

## API Endpoints

- `GET /api/repos` - List repositories
- `POST /api/repos` - Create repository
- `DELETE /api/delete?repo=<name>` - Delete repository

## Local Development

```bash
export GITHUB_TOKEN=your_token_here
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python app.py
```

Visit http://localhost:5000
