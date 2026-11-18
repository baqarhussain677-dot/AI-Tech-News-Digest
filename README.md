# Automated Tech News Digest (n8n)

An automated n8n workflow that collects daily tech news, filters relevant topics, saves a log, and sends email alerts.

## How It Works
1. **Schedule Trigger:** Runs the workflow automatically on a set schedule.
2. **HTTP Request:** Fetches the latest 50 stories from the HackerNews API.
3. **Split Out:** Splits the fetched news array into individual story items.
4. **Filter:** Keeps only stories containing specific keywords (`AI`, `Python`, `Cybersecurity`).
5. **Google Sheets:** Appends the filtered articles (Date, Title, URL, Author) into a Google Sheet log.
6. **Gmail:** Sends the filtered news directly to Gmail.
