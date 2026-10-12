# Website pages

## Revenue Leak Calculator (`revenue-leak-calculator/`)

A free calculator for the website. Visitors enter a few numbers and see an estimate of what they lose each month to missed calls, slow follow-up, no-shows and past customers. Then they can request a free 90-Day Double-Revenue Plan.

| File | Use it for |
|---|---|
| `calculator.html` | Paste into a custom HTML/code block on any page (GoHighLevel, WordPress, Webflow, Squarespace) |
| `index.html` | A complete standalone page, if you host it as its own URL or put it in an iframe |

### Settings

All settings are attributes on the `<div class="rlc" …>` line near the top of `calculator.html`:

| Attribute | What to put | Example |
|---|---|---|
| `data-webhook` | The address that receives each plan request as JSON | Your GoHighLevel inbound webhook URL |
| `data-booking` | Calendar link shown after someone submits | Your GHL booking page |
| `data-brand` | Your agency name (used in the consent text) | `Ironclad Growth` |
| `data-lock="light"` | Keeps it light even in dark mode. Delete to follow the visitor's device. | — |

Until `data-webhook` is set, the form shows "This form isn't connected yet" instead of pretending to send.

### Add it to a GoHighLevel site

GHL renames menus from time to time, so the labels below may differ slightly in your account.

1. In GHL go to **Automation → Workflows → Create workflow**, add the trigger **Inbound Webhook**, and copy its URL.
2. Paste that URL into `data-webhook` in `calculator.html`.
3. Open your site page in **Sites → Websites/Funnels**, add a **Custom JS/HTML** element, and paste the whole contents of `calculator.html`.
4. Submit a test entry, then in the workflow click **Fetch sample request** and map the fields (`name`, `email`, `phone`, `business`, `website`, `estimate_monthly`, etc.) to a **Create/Update Contact** action.
5. Add the rest of the workflow: tag `calculator-lead`, create an opportunity in the pipeline at **MQL**, notify the setter, and send the confirmation email/text.

The payload also includes everything the visitor entered and the estimate for each leak, so the setter can open the call with their own numbers.

### Notes

- The estimate is labeled as an estimate, and the assumptions are visible and editable. Keep it that way: it protects you under FTC rules on earnings claims.
- The consent checkbox covers calls and texts (TCPA). Only text or auto-dial people who ticked it.
- Industry presets and assumptions are in the `PRESETS` and `SPEED_LOSS` objects in the script. Adjust them once you have real numbers from your audits.

## Guarantee terms (`guarantee/index.html`)

The public "How our guarantee works" page. Before publishing:

1. Replace every placeholder: `[Brand]`, `[contact email]`, `[Legal entity]`, `[State]`, `[date]`.
2. Make sure the terms match your signed service agreement word for word on the numbers (14 days, 90 days, ad spend minimums, conditions).
3. Have a US attorney review both documents.
4. Link to this page from the calculator results, your sales proposal and email 3 of the cold sequence.
