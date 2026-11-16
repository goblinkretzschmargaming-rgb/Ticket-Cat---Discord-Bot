# Ticket Cat — Terms of Service

**Effective date:** 16 November 2026  
**Last updated:** 16 November 2026

These Terms of Service ("Terms") govern access to and use of the **Ticket Cat** Discord bot ("Ticket Cat", "the Bot", "we", "us", or "our"). By inviting, configuring, or using the Bot, you agree to these Terms. If you do not agree, do not use the Bot.

> **Important:** The public operator name supplied for this draft is **odsbud** (Discord). The operator's full legal name and postal contact address have not been supplied; add any details required by applicable law before publication. This is a general draft, not legal advice.

## 1. What Ticket Cat does

Ticket Cat is a Discord support and ticket-management bot. Depending on the version and server configuration, it may provide:
- Ticket creation, categories, ticket limits, and private ticket channels.
- Ticket claiming, staff-role routing, transfers, priorities, and closure reasons.
- Ticket transcripts, audit logs, and direct-message closure receipts.
- Optional star ratings and written feedback.
- Blacklisting and abuse-prevention features.
- Auto-responses, support statistics, dashboards, and administrative setup tools.

Features depend on Discord permissions, role hierarchy, server configuration, and the Bot's availability.

## 2. Eligibility and Discord

You must meet the minimum age requirements applicable to your use of Discord and comply with Discord's Terms of Service, Community Guidelines, and other applicable policies. Ticket Cat is an independent third-party bot and is not owned, operated, or endorsed by Discord unless expressly stated otherwise. Discord's own terms and privacy policy apply to your use of Discord.

## 3. Acceptable use

You must not use Ticket Cat to:
- Spam, flood, or repeatedly create tickets to disrupt support or evade configured limits.
- Harass, threaten, abuse, or discriminate against users or staff.
- Submit malicious files, harmful links, or content intended to compromise users, servers, or systems.
- Impersonate another person or knowingly submit deceptive information.
- Exploit bugs, bypass permissions, interfere with the Bot, or attempt unauthorised access.
- Violate applicable law, Discord policies, or the rules of the server using the Bot.
- Manipulate ratings, feedback, statistics, blacklists, or other Bot features.

When opening a ticket, provide a clear topic and relevant details, avoid duplicate tickets, and communicate respectfully. Do not submit passwords, payment-card details, or other highly sensitive information unless a secure process has specifically been provided.

## 4. Server owner and administrator responsibilities

The server owner and administrators are responsible for:
- Deciding whether to invite and use Ticket Cat.
- Configuring categories, ticket limits, staff roles, channel permissions, log channels, and transcript channels.
- Ensuring only appropriate people can access private ticket channels, logs, and transcripts.
- Informing server members about the server's ticket-handling and privacy practices where required.
- Ensuring their use of the Bot complies with applicable laws, Discord policies, and their own server rules.

Incorrect role hierarchy or channel permissions can prevent features from working or expose ticket information to unintended people. Administrators should review permissions after setup and whenever roles or categories change.

## 5. Tickets, transcripts, logs, and ratings

Ticket content is supplied by users and may be visible to the ticket creator, authorised staff, and server administrators. The purpose of a transcript is to preserve a record of what was said in the support conversation. This allows the relevant server's authorised staff and administrators to review the interaction, assess professionalism and support quality, determine whether the user received the help they needed, and investigate complaints, disputes, or unresolved matters. Ticket Cat is not intended to use transcript contents for unrelated profiling or to collect information beyond what is needed to operate and document the ticketing service.

The current transcript implementation processes up to 500 channel messages, excludes bot-authored messages, and represents image attachments as [Image] and other attachments by filename; it does not embed the actual attachment contents. Transcripts may be uploaded to the configured transcript channel or, if unavailable, the log channel. The transcript is therefore a limited text record of the ticket channel, not necessarily a complete copy of every message and attachment.

Closing a ticket does not necessarily erase its record. The current implementation marks a deleted ticket as Deleted in the database while retaining its ticket row; transcript files and log messages may also remain in Discord. Server administrators should manage channel access and retention appropriately.

If ratings are enabled, a ticket creator may receive a direct message inviting them to submit a 1–5 star rating and optional feedback. Staff accounts identified by the Bot's support-role or permission check are excluded from the rating controls.

## 6. Enforcement and restrictions

The Bot or server administrators may restrict ticket access, close tickets, blacklist users, or disable features where reasonably necessary to address abuse, protect a community or the service, enforce server rules, or comply with law. Server administrators control their own servers and may remove the Bot or change its permissions at any time.

## 7. User content

You retain whatever rights you have in content you submit. You are responsible for ensuring that you have the rights and permissions needed to submit it.

You permit the Bot operator to process and display that content as reasonably necessary to provide, secure, and maintain the Bot's ticketing features, including routing tickets, displaying them to authorised staff, and creating transcripts and logs. This does not transfer ownership of your content to the operator.

## 8. Availability and changes

Ticket Cat is provided on an as-available basis. We do not guarantee uninterrupted or error-free operation, compatibility with every server configuration, a particular support response time, or permanent availability of any feature. We may modify, suspend, or discontinue the Bot or any feature for maintenance, security, operational, or legal reasons.

## 9. Third-party services

Ticket Cat depends on Discord and may depend on third-party hosting or infrastructure services. Those services are governed by their own terms and policies. To the extent permitted by law, the Bot operator is not responsible for third-party outages or changes outside its reasonable control.

## 10. Disclaimers

To the extent permitted by applicable law, Ticket Cat is provided without warranties, express or implied. We do not warrant that the Bot will meet every user's requirements, that data will never be lost, or that every ticket or transcript will always be available.

Nothing in these Terms excludes or limits a right or remedy that cannot lawfully be excluded or limited.

## 11. Limitation of liability

To the maximum extent permitted by applicable law, the Bot operator will not be liable for indirect, incidental, special, consequential, or punitive losses, or for loss of profits, goodwill, data, or business opportunities arising from use of or inability to use Ticket Cat.

Nothing in these Terms limits liability where such limitation is prohibited by law. Any limitation in this section applies only to the extent legally enforceable.

## 12. Privacy

The Ticket Cat Privacy Policy explains how information may be processed in connection with the Bot. It is available at https://github.com/goblinkretzschmargaming-rgb/Ticket-Cat---Discord-Bot/blob/main/docs/PRIVACY_POLICY.md and forms part of the information governing use of Ticket Cat.

## 13. Changes to these Terms

We may revise these Terms as the Bot or applicable requirements change. We will publish the updated version with a revised "Last updated" date. Continued use after changes take effect constitutes acceptance only to the extent permitted by applicable law.

## 14. Governing law and contact

- **Operator / public name:** odsbud (Discord)
- **Governing law:** The laws of Denmark.
- **Jurisdiction:** The competent courts in Denmark, subject to any mandatory rules that give consumers or other users the right to bring proceedings elsewhere.
- **Contact email:** odsbudz@gmail.com

The operator is based in Denmark. The operator's full legal name and postal address have not been supplied in this draft; these should be added where required by applicable law. Nothing in this section removes any mandatory consumer or data-protection rights that apply to you.

---

*This document is a general draft based on the Ticket Cat source code supplied to the drafter. Complete the placeholders and obtain appropriate legal review before publication, especially if the Bot is offered publicly or to users in multiple countries.*
