**Smart Company News Chatbot**

What is this?

This is a **smart chatbot** that gives you the **latest news about any company** in real time. You just type the company name (or multiple names), and it will:

* Search the internet for fresh news,
* Pick the most relevant articles,
* Summarize them for you using AI,
* And talk like a normal assistant!

It’s like asking ChatGPT, *“What’s new with Google and Tesla?”* — but this chatbot uses **only free tools**, and **no paid APIs**.


What can it do?

✅ Take 1 or more company names from your message
✅ Search **Bing News** live for articles (no APIs used)
✅ Scrape real articles and read their content
✅ Use a **free AI model (T5-small)** to summarize the news
✅ Let you choose how you want the response:

* Formal business summary
* Quick bullet points
* Friendly, casual tone

✅ Handle greetings like “Hi” or “How are you?”
✅ Detect invalid or misspelled company names
✅ Show clean output with links to the source

How does it work?

1. You type:
   `What’s the latest news about Amazon and Tesla?`

2. The bot:

   * Finds company names in your message
   * Searches **Bing News**
   * Filters out unrelated or fake results
   * Visits the article pages and extracts the content
   * Uses the **T5-small AI model** to create short summaries
   * Formats the answer in your selected style

3. You get a clean reply with summaries and links!

Tech Used
* **Streamlit** – Chat-style web interface
* **Requests + BeautifulSoup** – For scraping articles from Bing
* **T5-small (HuggingFace Transformers)** – For text summarization
* **Python (Concurrent Futures)** – For fast, parallel scraping
* **No paid APIs** – 100% free and open-source tools only

Challenges Solved
* No APIs: Built real-time scraping instead
* Invalid results: Added a check to avoid unrelated news
* Short content: Used fallback snippets when full text wasn’t available
* Slow speed: Made scraping and summarizing run in parallel
* Casual talk: Responds to greetings like a real chatbot

