# WC 2026 Predictions

A predictions tournament app for the 2026 FIFA World Cup.

## Setup

### 1. Install dependencies
```
npm install
```

### 2. Environment variables
Create a `.env` file in the root (already included) with your Supabase credentials:
```
REACT_APP_SUPABASE_URL=https://wrhrdxtrxntewfxjbnsm.supabase.co
REACT_APP_SUPABASE_ANON_KEY=your_anon_key
```

### 3. Run locally
```
npm start
```

### 4. Deploy to Vercel
- Push to GitHub
- Import repo in Vercel
- Add environment variables in Vercel dashboard
- Deploy

## Adding new users
Run this SQL in the Supabase SQL editor:
```sql
insert into users (username, password_hash, is_admin) values ('newname', 'theirpassword', false);
```

## Scoring
- Correct result (win/draw/loss): 3 points
- Correct home score: +1 point  
- Correct away score: +1 point
- Maximum per match: 5 points
