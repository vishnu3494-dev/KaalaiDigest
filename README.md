# KaalaiDigest
This App Script in combination with Telegram bot and Groq Ai provides daily extraordinary morning news brief , Challenges different parts of your brain every 40 min and much more.

/**
 * ZERO-COST DAILY COGNITIVE AI AGENT — Groq Cloud edition
 *
 * LLM ............ openai/gpt-oss-120b (fallback: openai/gpt-oss-20b)
 * Speech-to-text . whisper-large-v3-turbo on Groq (for Telegram voice notes)
 * News grounding . free Google News / YouTube RSS feeds (the LLM has no web access)
 * Delivery ....... Telegram bot hosted on Google Apps Script
 *
 * Features
 * 1) 7:30 AM IST  Morning digest + active-recall quiz + mind-body protocol
 * 2) Every 30 min (10:00 AM - 9:30 PM IST)  15-minute whole-brain break
 * 3) 10:00 PM IST Journal, speech task, Socratic question, invention masterclass
 * 4) Two-way chat via webhook: quiz answers, debates, voice-note speech analysis
 *
 * ONE-TIME SETUP
 * 1) Project Settings -> Script Properties -> add:
 *      GROQ_API_KEY, TELEGRAM_BOT_TOKEN, TELEGRAM_CHAT_ID
 * 2) Run listGroqModels() to see which model IDs your Groq key can use (fix CONFIG.MODEL if needed),
 *    then run testSetup() once and approve the permissions.
 * 3) Deploy -> New deployment -> Web app (Execute as: Me, Who has access: Anyone).
 *    Add the /exec URL as Script Property WEBAPP_URL, then run setTelegramWebhook().
 * 4) Run setupDailyTriggers() once.
 *
 * NEVER paste keys or tokens into this file.
 */

