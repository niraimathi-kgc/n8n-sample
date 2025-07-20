# n8n Sample Workflow

This repository contains a sample workflow for [n8n](https://n8n.io/), an extendable workflow automation tool. The workflow demonstrates how to automate the process of fetching DevOps news from an RSS feed and distributing it via Discord and email.

## Workflow Overview

The workflow performs the following steps:

1. **Manual or Scheduled Trigger**
   - The workflow can be started manually or on a schedule (e.g., daily at 1 AM).

2. **RSS Feed Read**
   - Fetches the latest articles from the [DevOps.com RSS feed](https://devops.com/feed/).

3. **Limit**
   - Restricts the number of articles processed (e.g., to the most recent one).

4. **Edit Fields**
   - Maps and formats the RSS data fields for further use.

5. **Discord Notification**
   - Sends a formatted message to a Discord channel using a webhook, sharing the latest article details.

6. **Email Notification**
   - Sends a styled HTML email with the article's content to a specified recipient.

## Nodes Used
- **Manual Trigger**: Starts the workflow manually.
- **Schedule Trigger**: Runs the workflow on a defined schedule.
- **RSS Feed Read**: Fetches articles from an RSS feed.
- **Limit**: Restricts the number of items processed.
- **Set (Edit Fields)**: Maps and formats data fields.
- **Discord**: Sends messages to a Discord channel via webhook.
- **Email Send**: Sends emails using SMTP.

## How It Works
- The workflow can be triggered manually or automatically on a schedule.
- It fetches the latest news articles from DevOps.com.
- Only the most recent article is processed.
- The article's details are formatted and sent to both a Discord channel and an email address.

## Customization
- **RSS Feed URL**: Change the URL in the RSS Feed Read node to fetch from a different source.
- **Discord Webhook**: Update the Discord node with your own webhook credentials.
- **Email Settings**: Configure the Email Send node with your SMTP credentials and recipient details.

## Requirements
- An [n8n](https://n8n.io/) instance (cloud or self-hosted)
- Valid Discord webhook credentials
- SMTP credentials for sending emails

## Usage
1. Import the `sample-workflow.json` file into your n8n instance.
2. Set up the required credentials for Discord and SMTP.
3. Activate the workflow or run it manually to test.

---

**Author:** Your Name

This workflow is for demonstration and learning purposes. Feel free to modify and extend it for your own automation needs!
