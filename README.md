# Lead Management Automation

## Overview

An automated lead management system built with n8n.

The workflow receives customer inquiries through an HTTP Webhook, validates and cleans incoming data, stores leads in Google Sheets, and sends Telegram notifications.

## Architecture

Webhook → Edit Fields → IF → Google Sheets → Telegram → Respond to Webhook.

Invalid requests are handled through a separate validation branch.

## Features

- HTTP POST Webhook integration
- Data cleaning and normalization
- Email validation using Regular Expressions
- Conditional workflow branching
- Automatic lead creation and updating by email
- Google Sheets integration
- Telegram Bot API notifications
- HTTP 201 and 400 responses

## Technologies

- n8n
- Google Sheets
- Telegram Bot API
- JSON
- HTTP
- JavaScript Expressions
- Regular Expressions

## Testing

The workflow was tested with:
- Valid customer submissions
- Duplicate email addresses
- Invalid email formats


## Purpose

This project demonstrates workflow automation, API integrations, data validation, and basic CRM functionality.

**Note:** Credentials and sensitive information are excluded from the repository.
