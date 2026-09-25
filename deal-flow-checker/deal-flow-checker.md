# Project Name: Deal Flow Checker

## What It Does

Deal Flow Checker is an n8n automation that monitors incoming deal-flow emails in Gmail, analyzes the business opportunities mentioned in each email, checks them against predefined acquisition criteria, and sends qualified opportunities directly to Slack for review.

## Problem Before

Deal-flow emails often contain long, unstructured descriptions of businesses, financial metrics, links, and acquisition details.

Reviewing each email manually can be slow and inconsistent, especially when the team needs to quickly determine whether a company fits specific acquisition criteria.

Without automation, valuable opportunities may be missed, delayed, or buried in a crowded inbox.

## What Jan Built

Jan built an AI-powered n8n workflow that starts with a Gmail trigger and extracts the sender and email body for analysis.

The workflow first uses an AI agent to determine how many distinct businesses are mentioned in the email. A JavaScript code node then parses the AI output into a usable number, allowing the workflow to branch intelligently.

If the email contains one business, the workflow sends it to a **Single Business Analyst** agent. If the email contains multiple businesses, it routes the content to a **Multiple Business Analyzer** agent.

These agents evaluate each business against acquisition criteria, including business type, industry, revenue, EBITDA, location, and years active.

The workflow also includes a link extraction tool to identify the most relevant access link for the business opportunity, structured output parsers to keep results clean, conditional logic to separate qualified and unqualified opportunities, and Slack notifications to alert the team when a deal should be pursued.

## Tools Used

* n8n
* Gmail Trigger
* OpenAI GPT-4o Mini
* GPT-5 Mini
* LangChain AI Agent nodes
* Think Tool
* Structured Output Parsers
* Custom JavaScript Code node
* IF/Conditional Logic
* Set/Edit Fields nodes
* AI Link Extractor Tool
* Slack

## How Jan Helped the Employer or Client

Jan helped automate the first layer of investment and acquisition screening.

Instead of requiring someone to manually read every deal email, identify the businesses, check financial metrics, compare them against acquisition rules, and decide whether to alert the team, the workflow performs that process automatically.

This gave the team a faster way to surface qualified opportunities while filtering out deals that did not match the criteria.

It also reduced the chance of missing relevant opportunities hidden inside long emails or multi-business deal lists.

## Business Impact

This workflow saves time for executives, operators, or investment teams by reducing manual deal review.

It improves speed-to-decision by sending qualified opportunities directly to Slack, supports more consistent screening against acquisition criteria, and helps the team focus attention only on deals that are more likely to be worth pursuing.

## AI-Agent-Ready Summary

Jan built an n8n automation called **“Deal Flow Checker.”**

The workflow monitors Gmail for incoming deal-flow emails, extracts the sender and email body, counts how many businesses are mentioned, and routes the email into either a single-business or multiple-business analysis path.

The workflow uses AI agents to evaluate each business against acquisition criteria involving industry, business type, revenue, EBITDA, location, and years active.

Qualified opportunities are sent to Slack for team review, while unqualified deals are ignored.

This project demonstrates Jan’s ability to build AI-powered business analysis workflows that combine email automation, investment criteria evaluation, structured AI outputs, conditional routing, and real-time team notifications.
