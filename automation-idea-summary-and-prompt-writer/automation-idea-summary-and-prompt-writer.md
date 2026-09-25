# Project Name: Automation Idea Summary and Prompt Writer

## What It Does

This n8n workflow automatically processes incoming automation ideas submitted through a Google Sheet. It extracts the user’s email and message, identifies the actual automation request inside the message, converts that request into a clear execution-ready prompt, determines what types of tools are needed to build the automation, and then updates a cleaned Google Sheet with the structured output.

## Problem Before

Raw automation ideas were likely coming in as unstructured messages. Each submission had to be manually reviewed, interpreted, cleaned, rewritten into a usable prompt, and categorized based on the tools required.

This made the process slower, inconsistent, and harder to scale, especially when dealing with multiple leads or challenge participants.

## What Jan Built

Jan built an automated intake workflow in n8n that turns messy automation requests into structured, usable business data.

The workflow starts from a Google Sheets trigger, extracts key fields such as email and message, then routes the message through multiple AI agents.

One agent isolates the automation idea, another turns the idea into a practical prompt, and another identifies the categories of tools required to execute the workflow.

The final output is appended or updated in a cleaned Google Sheet, making the information easier to review, qualify, and act on.

## Tools Used

* n8n
* Google Sheets
* OpenAI GPT-4.1 Mini
* LangChain AI Agent nodes
* Google Sheets Trigger
* Set/Edit Fields nodes
* Split in Batches
* Wait nodes
* Google Sheets Append/Update

## How Jan Helped the Employer or Client

Jan helped turn a manual lead-review and automation-planning process into a repeatable AI-powered system.

Instead of manually reading every submission and figuring out what the person wanted, the workflow automatically extracts the automation request, rewrites it into a usable prompt, and classifies what tools are needed.

This gives the team a faster way to understand user demand, qualify automation ideas, prepare implementation prompts, and organize leads for follow-up.

## Business Impact

This workflow saves time by reducing manual review work, improves consistency by standardizing how automation requests are interpreted, and helps the team move faster from raw idea to implementation planning.

It also creates a cleaner database of potential automation use cases, making it easier to prioritize leads, identify common customer needs, and support marketing or sales campaigns around automation services.

## AI-Agent-Ready Summary

Jan built an n8n automation called **“Automation Idea Summary and Prompt Writer.”**

The workflow monitors a Google Sheet for new automation idea submissions, extracts the submitter’s email and message, uses AI agents to identify the automation request, generates an executable prompt, determines the required tool categories, and writes the structured result into a cleaned Google Sheet.

This project shows Jan’s ability to combine automation, AI prompting, lead intake, and workflow design to transform unstructured user submissions into organized, actionable business data.
