# Ticket Cat — Privacy Policy

**Effective date:** 16 November 2026  
**Last updated:** 16 November 2026

This Privacy Policy explains how the operator of **Ticket Cat** ("Ticket Cat", "we", "us", or "our") handles information when you use the Ticket Cat Discord bot.

> **Important:** The public operator name supplied for this draft is **odsbud** (Discord). The operator's full legal name and postal contact address have not been supplied. Add any identity/contact details required by applicable law before publication. This is a general draft, not legal advice.

## 1. Who is responsible?

- **Operator / public name:** odsbud (Discord)
- **Country:** Denmark
- **Privacy contact email:** odsbudz@gmail.com

The Bot is developed and operated by the individual using the public name **odsbud**. The operator's full legal name and postal address have not been provided in this draft; these should be added if required to identify the data controller adequately under applicable law. Contact **odsbudz@gmail.com** with privacy questions or requests.

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

Ticket records and transcripts are intended to document the support interaction that took place in a ticket. The transcript is a record of the conversation in the ticket channel, so the relevant server's authorised staff and administrators can review what was said, assess whether support was handled professionally, understand whether the user received the help they needed, and follow up on complaints, disputes, or unresolved issues. The Bot does not need to add unrelated personal information to the transcript for these purposes.

We also use the associated information to:
- Create, route, assign, manage, reopen, close, and delete ticket channels.
- Enforce ticket limits and server-specific blacklist rules.
- Apply category, staff-role, and channel permissions.
- Detect configured auto-responder phrases within ticket messages.
- Record support actions and generate audit logs and closure receipts.
- Collect optional ratings and feedback and calculate support statistics.
- Maintain, troubleshoot, secure, and improve the Bot.

The transcript is a representation of the messages available in the ticket channel when it is generated, not a guarantee that every message or attachment is reproduced in full. As implemented, it retrieves up to 500 messages, excludes bot-authored messages, and represents attachments by a short label or filename rather than copying their contents.

## 4. Legal basis and applicable data-protection law

The operator is based in Denmark. Where the GDPR applies, each processing purpose must have an appropriate legal basis under Article 6 and the operator must be able to explain that basis. The precise allocation of controller and processor responsibilities may depend on how a particular Discord server uses the Bot: server owners or administrators decide why their support tickets are collected and which staff can access them, while the Bot operator develops and operates the software and determines certain technical means and service operations.

The operator must document the appropriate legal basis for each processing activity before publication and use. Legitimate interests may be relevant for operating, securing, and maintaining the Bot, but this requires an actual assessment and does not automatically justify every use or indefinite retention. Optional ratings and feedback should not be described as consent-based unless a valid consent process is actually used.

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

**Current practice: ticket database records are retained indefinitely.** The operator has stated that ticket records are intended to remain available without a fixed expiry. The supplied code has no automatic retention period, scheduled purge, or per-server deletion command.

The SQLite database is a single database file (ticketcat.db) containing records for multiple Discord servers, distinguished by each record's server (guild) ID; it is not a separate database file controlled independently by each Discord server. Server administrators configure their own ticket channels, log channels, transcript channels, and access permissions, but the database retention described here is managed by the Bot operator. Ticket metadata, close reasons, ratings, feedback, blacklist entries, and statistics remain in that database unless they are manually removed or the relevant database data/file is otherwise deleted.

When a ticket channel is deleted through the Bot, the ticket's database row is retained and its status is changed to Deleted. Deleting the Discord channel therefore does not itself erase the database record. Transcript attachments and log messages uploaded to Discord may also remain there until deleted from Discord.

The operator has not confirmed backup retention, host-level logs, or a formal manual deletion workflow. Indefinite retention must be reviewed against the purposes for which the information is held and applicable data-protection requirements. Under the GDPR storage-limitation principle, personal data should not be kept longer than necessary; a blanket promise to keep identifiable ticket records forever may not be lawful in every circumstance. Requests for erasure or restriction will be assessed under applicable law, and records will be deleted where required. Contact **odsbudz@gmail.com** to make a request.

## 7. Your privacy rights and requests

Depending on your location and applicable law, you may have rights to request access, correction, deletion, restriction, or portability of personal information, or to object to certain processing. Where processing relies on consent, you may be able to withdraw it.

Contact **odsbudz@gmail.com** with your request and enough information to identify the relevant server and ticket. Do not send passwords or sensitive identity documents through an ordinary Discord ticket. We may need to verify your request and may retain some information where permitted or required by law.

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

Privacy requests and questions: **odsbudz@gmail.com**.

If you are in Denmark and believe personal data has been processed in breach of applicable data-protection law, you may lodge a complaint with the Danish Data Protection Agency (Datatilsynet): https://www.datatilsynet.dk/english.

---

*This policy is based on the Ticket Cat source code supplied to the drafter. It must be checked against the live deployment and the operator's actual hosting, security, retention, and deletion practices before publication.*
