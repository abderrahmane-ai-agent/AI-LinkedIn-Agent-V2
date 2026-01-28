# AI-LinkedIn-Agent-V2
AI-LinkedIn-Agent-V2: Multi-Agent Research & Content Engine
Executive Summary

This is a high-performance autonomous agent system that uses a chained-LLM architecture to transform raw email topics into research-backed LinkedIn posts. Unlike Level 1, this version uses a dedicated Researcher Brain to validate facts before the Writer Brain drafts the content.

🏗 The Stack

Orchestration: Make.com

Intelligence: * Brain #1 (Researcher): groq/compound-mini (Web-search enabled)

Brain #2 (Ghostwriter): llama-3.1-8b-instant (Low-latency inference)

Trigger: Gmail API (Watch Emails)

Storage: Google Sheets (Data Archive) & GitHub (Execution Logs)

🧠 Logic Flow (Level 2 Upgrade)

Watch: Monitors Gmail for specific subject lines.

Research (Brain #1): Groq searches the web to find 3-5 facts about the topic and returns cited sources.

Sleep (Safety): A 10-30 second delay ensures we stay within Free Tier Rate Limits (TPM/RPD).

Transform (Brain #2): Groq takes the research and drafts a "Pattern Interrupt" LinkedIn post.

Log: Parallel updates to Google Sheets for tracking and GitHub for version-controlled logs.

📈 Contribution to Goal

"Transitioning into the top 1% of AI practitioners by 2026."

