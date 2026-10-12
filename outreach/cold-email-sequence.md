# Cold Email Sequence: Revenue Leak Audit

Four emails over 12 days to US local service business owners. The goal of every email is a **reply**, not a click. The offer is the free Revenue Leak Audit; the guarantee comes in email 3.

## Before you send

- **Sending setup:** separate domains (never your main one), 2–3 inboxes each, SPF/DKIM/DMARC set, warmed for 14–21 days, 30–40 sends per inbox per day.
- **List:** verified emails only. One trade per campaign, so the copy can name it.
- **Format:** plain text, under 100 words, no images, no links in email 1, no attachments.
- **Stop rules:** any reply (positive, negative or "remove me") stops the sequence for that contact. Honor unsubscribes immediately.
- **Footer (CAN-SPAM), on every email:**

  ```
  [Brand] · [physical mailing address]
  Not relevant? Reply "no thanks" and I won't email again.
  ```

## Variables

| Variable | Example | Source |
|---|---|---|
| `{{FirstName}}` | Mike | Apollo / manual research |
| `{{Company}}` | Rivera Heating & Air | Google Maps |
| `{{City}}` | Plano | Google Maps |
| `{{industry}}` | HVAC | Campaign |
| `{{service}}` | AC repair | Their website |
| `{{Signal}}` | One of the first lines below | Research step |
| `{{YourName}}` | Sam | Sender |

### First-line options (`{{Signal}}`)

Use the strongest true signal you found. Never invent one.

| Signal | First line |
|---|---|
| Missed mystery call | I called {{Company}} after 6pm last Tuesday about {{service}}. It went to voicemail and nobody texted back. |
| Running ads | Saw {{Company}} is running ads on Facebook right now. Nice creative. |
| Fewer reviews than competitors | {{Company}} has {{reviews}} Google reviews. The top {{industry}} shop in {{City}} has {{competitor_reviews}}. |
| Hiring front desk | Saw you're hiring a front desk person. Usually means the phones are getting busy. |
| Slow web form | I filled out the form on your site on {{day}} and heard back {{time}} later. |

---

## Email 1 · Day 1 · The leak

**Subject (A/B test):**
- A: `{{Company}} after 6pm`
- B: `missed calls at {{Company}}`

```
Hi {{FirstName}},

{{Signal}}

For most {{industry}} owners in {{City}}, that's where a chunk of new customers go to whoever answers first.

I put together a short audit showing what that's likely costing you each month, plus two other leaks I found. Want me to send it over?

{{YourName}}
```

> Why it works: a personal, true observation, a problem in their money, and a free thing with a one-word reply ("sure"). *$100M Leads*: personalize, then give big fast value.

---

## Email 2 · Day 3 · Proof

**Subject:** `re: {{Company}} after 6pm` (same thread)

**Version with a case study (use once you have one):**

```
{{FirstName}}, quick follow-up.

We set this up for {{CaseStudyBusiness}}, a {{industry}} company in {{CaseStudyCity}}. Every call now gets answered, missed calls get a text back in under a minute, and old customers get a comeback offer every quarter.

First 90 days: {{CaseStudyResult}}.

Worth 15 minutes to see what the same setup would do for {{Company}}?

{{YourName}}
```

**Version before you have case studies:**

```
{{FirstName}}, quick follow-up.

Here's what we'd set up for {{Company}}: an AI receptionist that answers every call 24/7, a text back to every missed caller within 60 seconds, and an automatic follow-up on every form lead until they book.

Most owners see recovered bookings in the first week.

Want me to send the audit so you can see your numbers first?

{{YourName}}
```

> Only state results you can prove. Remove "Most owners see…" until your own clients have done it.

---

## Email 3 · Day 7 · The guarantee

**Subject (A/B test the size of the promise):**
- A: `double {{Company}}'s revenue?`
- B: `$20k for {{Company}} in 90 days`

**Version A (double):**

```
{{FirstName}}, most agencies get paid whether you grow or not.

We work differently. If {{Company}}'s revenue hasn't doubled within 90 days of your system going live, we keep working with no monthly fee until it has. The full terms are on our site, nothing hidden.

We only take businesses where the audit shows it's realistic, and a few per area.

Open to finding out if you qualify?

{{YourName}}
```

**Version B ($20k):**

```
{{FirstName}}, most agencies get paid whether you grow or not.

We work differently. If we don't add at least $20,000 in new revenue for {{Company}} within 90 days of your system going live, we keep working with no monthly fee until we do. The full terms are on our site.

We only take businesses where the audit shows it's realistic, and a few per area.

Open to finding out if you qualify?

{{YourName}}
```

> Send each version to ~500 prospects in the same trade. Keep the one with more **booked audits**, then watch which one produces fewer guarantee claims. *$100M Leads* advises the smallest promise that still closes.
>
> If you run version B, add a matching "$20,000 in new revenue" option to the guarantee terms page and contract before sending.

---

## Email 4 · Day 12 · Close the loop

**Subject:** `close the loop?`

```
{{FirstName}}, I'll stop emailing after this one.

If fixing missed calls and follow-up isn't a priority at {{Company}} right now, no problem.

If it is, just reply "audit" and I'll send yours over.

{{YourName}}
```

---

## After the sequence

- **No reply:** move to nurture. Re-contact in 3–6 months with a new first line. Circumstances change.
- **Calls:** the setter calls everyone who opened 2+ times, starting with "I sent you a couple of emails about your after-hours calls and wanted to follow up."
- **LinkedIn:** send a connection request on day 1 and a short DM on day 5 if they accepted.

## Reply templates

**Positive ("sure", "send it", "audit"):**

```
Great. I'll finish it this week. To make the numbers accurate, roughly how many calls do you get a month, and what's a typical new customer worth to you?

The quickest way to go through it is a 15-minute call. Does {{day}} at {{time}} or {{day2}} at {{time2}} work?
```

**"How much is it?":**

```
Fair question. It depends on what the audit shows. Plans start at $1,497/month, and the full system is $3,997/month plus ad spend, with the 90-day guarantee.

If the audit doesn't find real money you're losing, I won't pitch you anything. Want me to send it?
```

**"We already have an agency":**

```
Makes sense. Do they also handle missed calls, follow-up and bringing back past customers, or mainly ads? Most owners come to us with ads covered and leads falling through after. Happy to send the audit either way so you can compare.
```

**"Not interested" / "remove me":**

```
Understood, I've taken you off my list. All the best with {{Company}}.
```

(Then remove them from every campaign.)

## Weekly numbers to track

| Metric | Target to start | Action if below |
|---|---|---|
| Open rate | 40%+ | Check deliverability first, then test subject lines |
| Reply rate | 2–5% | Test first lines and the email 1 offer |
| Positive reply rate | 0.5–1.5% | Test the lead magnet (e.g. offer the free 14-day Missed-Call Rescue) |
| Positive replies that book | 50%+ | Reply faster: within 5 minutes during work hours |

Change **one thing per week**, log the result, and keep the winner.
