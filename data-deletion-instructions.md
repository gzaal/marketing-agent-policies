---
title: Data Deletion Instructions
permalink: /data-deletion/
---

# Data Deletion Instructions

Last updated: May 9, 2026

Marketing Agent is a private/beta application used to manage marketing workflows and connect approved Meta assets, including Facebook Pages and Instagram professional accounts.

This page explains how a user can request deletion of data associated with the Marketing Agent Meta app. It is intended for the Meta App Dashboard's Data Deletion Instructions URL when the application does not yet have a public production backend for an automated deletion callback.

## Remove Marketing Agent from Meta

You can revoke Marketing Agent's access from your Meta account at any time:

1. Open Facebook and go to Settings and privacy.
2. Select Settings.
3. Open Apps and Websites.
4. Find Marketing Agent.
5. Select Remove and confirm the removal.

This revokes future access to your Facebook and Instagram assets through Meta APIs. It does not necessarily delete data already stored by Marketing Agent, so use the request process below if you also want stored data removed.

## Request deletion from Marketing Agent

To request deletion of data held by Marketing Agent, contact the app operator through the contact method listed in the Meta App Dashboard or open a request at:

https://github.com/gzaal/marketing-agent-policies/issues

Do not include access tokens, passwords, private credentials, or sensitive personal data in a public GitHub issue. If the request requires private details, ask for a private contact channel first.

Please include enough information to identify the connection, such as the Meta app name, the Facebook Page name, the Instagram professional account username, and the email address used for the Marketing Agent workspace if applicable.

## What will be deleted

After a verified deletion request, Marketing Agent will delete or anonymize data associated with the relevant Meta connection, including:

- Meta OAuth access tokens and refresh-related credentials held by the app.
- Facebook Page IDs, Instagram professional account IDs, usernames, and connection records.
- Cached profile, Page, media, insight, scheduling, or publishing metadata retrieved through Meta APIs.
- Draft, scheduled, or unpublished content stored in Marketing Agent where it is tied to the requesting user or connected Meta asset.

Marketing Agent may retain limited records when required for security, fraud prevention, legal compliance, audit integrity, or backup recovery. Retained records will be minimized and disconnected from active Meta API access where practical.

## Timeline

Verified deletion requests are processed within 30 days unless a shorter period is required by applicable law. If more time is needed because the request is complex or cannot be verified, the app operator will provide an update.

## Data held by Meta

Deleting data from Marketing Agent does not delete data stored by Meta. To manage or delete data held by Facebook or Instagram, use the privacy and account settings provided by Meta.

## Automated callback

If Marketing Agent is later deployed with a public HTTPS backend, the app may use an automated Data Deletion Callback URL instead of this instructions page. The callback will verify Meta's signed request, delete associated data, and return a deletion status URL plus a confirmation code.
