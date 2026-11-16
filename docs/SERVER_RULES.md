# 🐾 Ticket Cat — Official Server & Support Ruleset

Welcome to **Ticket Cat**! These rules explain how members and support representatives should use the ticket system. Please read them carefully so every request can be handled fairly, safely, and efficiently.

## 1. User Ticket Guidelines

- **Active ticket limit:** Members may have a maximum of **3 active tickets** at a time, unless an administrator changes this limit with `/setup max_tickets`.
- **No limit evasion or spam:** Do not open multiple tickets to bypass the active-ticket limit or repeatedly create tickets for the same issue. Attempts to spam or evade the limit may result in an **automatic blacklist**.
- **Give useful details:** Choose a concise topic and provide a detailed description of the issue when opening a ticket. Include relevant information so staff can understand and investigate the request.
- **Be patient and respectful:** Support representatives may be handling other requests. Do not harass, pressure, or abuse staff.
- **Avoid duplicate tickets:** Do not create another ticket for an issue that is already being handled. Staff may transfer an existing ticket to the correct department when needed.

## 2. Staff & Representative Governance

- **Claim tickets:** A representative should use the **Claim Ticket** button to take responsibility for a ticket.
- **Department separation:** Staff should work within their assigned department roles and respect the separation of support responsibilities.
- **Transfer to the correct department:** Use `/ticket move` to transfer a ticket. The command moves the channel, updates role permissions/overwrites, and notifies the correct department.
- **Set ticket priority:** Use `/ticket priority` or **Quick Edit** to set a ticket to **Low**, **Normal**, **High**, or **Urgent**. Urgent safety-related matters should be pinned for visibility.
- **Close with a reason:** Close tickets using the close button or `/ticket close [reason]`. Provide a clear, specific reason. Standard reasons may include **Resolved**, **User Left**, **Duplicate**, **No Response**, or **Invalid Request**.
- **Transcripts and logs:** When a ticket is closed or deleted, a `.txt` transcript is generated in `#ticket-transcripts`, and a summary card is posted in `#ticket-logs`.

## 3. Audit Logging & Accountability

- **Immutable audit record:** The `#ticket-logs` card records the Ticket ID, Opened By, Closed By, Claimed By, Open Time, and Detailed Close Reason. These records are intended to preserve an accountable history of ticket handling.
- **Edit-reason permissions:** Only the representative who claimed the ticket or the representative who closed it may use **Edit Reason**.
- **Member closure receipt:** When a ticket is closed, the member receives a DM receipt containing the closure card and a **View Online Transcript** link.

## 4. Support Rating Policy

- **Member feedback:** Regular members receive a DM prompt after ticket closure asking them to rate their support experience from **1–5 stars**, with optional written feedback.
- **Staff exemption:** Support representatives cannot rate tickets. Their DM should state: “You cannot rate this ticket because you are a support representative...” and must not display rating buttons.
- **View metrics:** Use `/stats user` for individual statistics and `/stats global` for global support statistics.

## 5. Security, Blacklisting & Enforcement

- **Blacklist abusive users:** Use `/blacklist add [user] [reason]` to block a user from opening new tickets across all categories. This may be used for abuse, malicious attachments, harassment, or other serious misuse of the support system.
- **Ticket Cat role position:** In **Server Settings → Roles**, place the **Ticket Cat** role above the staff roles it needs to manage. Discord role hierarchy affects the bot's ability to manage permissions and roles.

---

By using the Ticket Cat support system, members and representatives agree to follow these rules. Staff may take appropriate action to protect the community and keep support operations organized, safe, and fair.
