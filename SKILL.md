---
name: inbox-triage-text
description: Texts the student only the emails that need action or a reply, ranked by the student's own priorities, and calls about anything due in under 24 hours. Use when the student says their inbox is out of control, they are afraid of missing an important email, or they want a nightly check for emails that need a response.
---

# Inbox Triage Text

This Skill uses only Cubbie's built-in capabilities. It has no scripts.

## When to use

- "I have 200 unread emails, what actually matters?"
- "Text me if something in my inbox needs me to act or reply."
- "Set up a nightly check for important email."
- "Redo my categories" or "change my ranking."

Do not use it to find one specific email, write a new email or track Canvas assignments.

## Steps

1. Check Cubbie's **Memory** for a saved ranking. If there is none, read the last 72 hours of email with Cubbie's **Email events** capability (and **Gmail** if that is what is connected), read and unread, leaving out Canvas notification emails.
   Sort it into the categories this inbox actually has. Merge categories with fewer than 2 emails and keep the list to 12 or fewer.
   If email is not connected, tell the student, offer to connect it, and stop.
2. Text the numbered list with a rough count for each and ask the student to rank it, most important first, and to leave out any they never want texts about.
   Say that after ranking you will check their email every night at 12 am and call them about anything due in under 24 hours, and that they can say "no nightly check".
   Categories not mentioned go to the bottom. Categories left out are never texted or called about.
   Save the ranking with **Memory**, then triage the same 72 hours right away. This first triage only texts and does not call.
3. For every triage, read email since the last check (the past 24 hours at night) and keep only emails that need the student to do something or reply, such as a direct question, a request for a form, document or payment, an account hold, a schedule change, or a request to confirm.
   Skip newsletters, mass announcements, receipts and Canvas notifications.
   Skip emails whose deadline has passed, unless it passed in the last 72 hours and nothing shows it was handled. Skip anything a later email shows is done.
   Mark each item Read or Unread. Never change an email's read status.
4. Order the list: anything due within 48 hours first, earliest first. Everything else follows the student's ranking, and within one category the earliest deadline goes first and emails with no deadline go last.
5. Text the top three, one short line each: who it is from, what is needed, and by when. If more were kept, say how many more and offer them.
   If an email fits no saved category, ask where the new category belongs, after the top three in the same text. Save the answer with **Memory** and do not ask again. If there is no answer, put it at the bottom and ask at the next check.
6. During a nightly check only, if a kept email is due in under 24 hours, call the student with Cubbie's phone call capability, once for all urgent items. Keep it short and spoken: who it is from, what is needed, and when it is due.
   This applies to every ranked category, including new ones, and never to categories the student left out. If the deadline is unclear, only text.
7. Offer to draft a reply for any item that needs one, with Cubbie's **Gmail** capability. Create a draft only and never send. Show it and let the student confirm or change it.
8. Save the time of this check with **Memory**. After the first triage, create a recurring check every night at 12 am in the student's time zone with Cubbie's **Reminders and scheduled check-ins** capability, unless they said "no nightly check". Tell the student in one line that it is set.
   Word it so it makes sense days later: "Run the inbox-triage-text Skill on the student's email from the past 24 hours, using the student's saved ranking. Text only emails that need action or a reply. Call about anything due in under 24 hours. If nothing needs action, send nothing."
9. When the student says "that one was not important", "you missed X" or "move recruiters up", update the saved ranking with **Memory** and say what changed in one line. Do not redo the setup unless they ask.

## Output

Reply in a few short lines of plain text, no Markdown, with the most urgent item first. For example: "2 emails need you: 1. Prof. Lee (Unread) asks which section you are in, reply by 9 am. 2. Immigration office (Read) needs your form, due Fri. Want me to draft both replies?"
Keep the full list for when the student asks.

## When something fails

- Nothing needs action: say "Nothing needs a reply right now" once, and in a nightly check stay silent and do not call.
- A call cannot be placed: send the urgent items as a text marked "Due soon".
- A draft cannot be created: say so and offer to show the text so the student can paste it.
- Memory cannot be saved: continue with the ranking from this chat and say it may need to be set again.
- Never guess a deadline. If an email has none, say "no deadline given".
