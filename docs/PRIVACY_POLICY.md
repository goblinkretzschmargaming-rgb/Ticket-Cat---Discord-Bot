# Ticket Cat — Privacy Policy

**Effective date:** 16 November 2026  
**Last updated:** 16 November 2026

This Privacy Policy explains how the operator of **Ticket Cat** ("Ticket Cat", "we", "us", or "our") handles information when you use the Ticket Cat Discord bot.

> **Publication checklist:** Replace all bracketed placeholders and verify the actual hosting, access, backup, and retention arrangements before publication. This is a general draft, not legal advice.

## 1. Who is responsible?

- **Operator / legal name:** [INSERT YOUR NAME OR ORGANISATION]
- **Privacy contact email:** [INSERT CONTACT EMAIL]
- **Country / business address (if applicable):** [INSERT DETAILS]

The operator identified above is responsible for deciding why and how Ticket Cat data is processed. Contact us at the email above with privacy questions or requests.

## 2. Information processed

Depending on the features enabled in a server and how people use them, Ticket Cat processes or may process:

### Discord identifiers and configuration
- Discord user IDs, server (guild) IDs, channel IDs, message IDs, and role IDs.
- Server settings, ticket categories, category descriptions, staff-role assignments, channel/category references, ticket limits, and tracked panel/statistics message information.
- Auto-responder trigger phrases and response text configured by server administrators.

### Ticket and support information
- Ticket ID, creator ID, ticket category/type, channel ID, topic, status, priority, timestamps, and first-response time.
- IDs of staff members who claim, close, or otherwise act on tickets.
- Close reasons, transfer/assignment information, and ticket audit/log references.
- Star ratings and optional written feedback submitted after a ticket closes.
- Blacklist user IDs, the recorded reason, the administrator who added the entry, and the time it was added.

### Messages and transcripts
Ticket Cat requests Discord's **Message Content** and **Server Members** privileged intents. Its ticket auto-responder checks message content in registered ticket channels for configured trigger phrases. The first staff response time may be recorded. Ticket content is also accessed when generating transcripts.

The transcript code currently retrieves up to **500 messages** from the ticket channel, excludes bot-authored messages, and writes human messages with timestamps, display names, and text. Image attachments are represented as [Image]; other attachments are represented by filename. The transcript is uploaded as a .txt attachment to the server's configured transcript channel, or the log channel as a fallback.

The SQLite ticket database stores ticket metadata, topics, reasons, ratings, and related identifiers; the code provided does not show ordinary ticket message bodies being written into SQLite as part of ticket creation. Message content can nevertheless remain in Discord channels and uploaded transcript attachments.

## 3. Purposes

We use this information to:
- Create, route, assign, manage, reopen, close, and delete ticket channels.
- Enforce ticket limits and server-specific blacklist rules.
- Apply category, staff-role, and channel permissions.
- Detect configured auto-responder phrases within ticket messages.
- Record support actions and generate audit logs, closure receipts, and transcripts.
- Collect optional ratings and feedback and calculate support statistics.
- Maintain, troubleshoot, secure, and improve the Bot.

## 4. Legal basis

Where applicable data-protection law requires a legal basis, the operator must identify and document one for each purpose. Depending on the deployment and context, possible bases may include legitimate interests in providing and securing a support system, steps taken at a server administrator's request, or consent where it is genuinely required. This draft does not determine the legal basis for the operator.

## 5. Where information is stored and who can access it

The supplied code uses a local **SQLite** database file named ticketcat.db. Ticket channels, log messages, and transcript attachments are also created or stored within Discord. The code does not identify the Bot's hosting provider, physical hosting location, backup service, or any additional infrastructure provider; those details must be added once confirmed.

Information may be accessible to:
- The ticket creator and other users explicitly given access to the ticket.
- Staff members whose roles are assigned to the relevant ticket category.
- Server administrators and people with sufficient Discord permissions.
- The Bot operator and authorised personnel with access to the Bot's host, database, or Discord account.
- Discord, as the platform through which the Bot operates.

Server administrators configure log and transcript channels and are responsible for their channel and role permissions. Discord independently processes information under its own terms and privacy policy.

## 6. Retention and deletion

The code provided does **not** implement a general automatic retention period or scheduled database purge.

When a ticket is deleted through the Bot, the ticket channel is deleted after the archive attempt, but the ticket's database row is retained and its status is changed to Deleted. The database schema also retains historical ticket records, ratings, feedback, and statistics. Deleting a ticket channel therefore does not itself erase its database record or the transcript attachment already uploaded to Discord.

The operator has not yet confirmed backup retention, host-level logs, or any manual deletion process. Before publication, specify:
- How long ticket records and feedback are kept.
- How long Discord transcripts and log messages are kept.
- Whether and how database backups are created and deleted.
- How to request deletion and what may need to be retained for legitimate or legal reasons.

**Retention schedule:** [INSERT ACTUAL RETENTION PERIODS AND DELETION PROCESS. Do not claim automatic deletion unless it is implemented.]

## 7. Your privacy rights and requests

Depending on your location and applicable law, you may have rights to request access, correction, deletion, restriction, or portability of personal information, or to object to certain processing. Where processing relies on consent, you may be able to withdraw it.

Contact **[INSERT CONTACT EMAIL]** with your request and enough information to identify the relevant server and ticket. Do not send passwords or sensitive identity documents through an ordinary Discord ticket. We may need to verify your request and may retain some information where permitted or required by law.

Server administrators can delete Discord channels or messages they control, but that may not delete the corresponding SQLite record, uploaded transcript, log, or backup. Requests concerning information held by Discord itself should also be directed to Discord.

## 8. Security

The code uses a local SQLite database and Discord permissions to support ticket access controls. The code alone does not establish the security of the hosting environment, operating-system permissions, secret storage, network configuration, backups, or staff access. The operator should document and maintain appropriate safeguards for the actual deployment. No online service can be guaranteed completely secure.

## 9. Children and age requirements

Ticket Cat is not intended to bypass Discord's minimum age requirements. Users must meet the age requirements applicable to their use of Discord. Server owners and administrators are responsible for ensuring their communities and use of the Bot comply with applicable law and Discord policies.

## 10. International transfers

Discord and any hosting or infrastructure providers may process information in countries other than the country where you live. The operator should identify the relevant providers, locations, and any required transfer safeguards before publication.

## 11. Changes

We may update this Policy when the Bot's features or data practices change. The latest version will be published at the policy URL with an updated date. Material changes should be communicated through an appropriate channel.

## 12. Contact

Privacy requests and questions: **[INSERT CONTACT EMAIL]**

---

*This policy is based on the Ticket Cat source code supplied to the drafter. It must be checked against the live deployment and the operator's actual hosting, security, retention, and deletion practices before publication.*
