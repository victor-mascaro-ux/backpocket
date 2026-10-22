# Backpocket · Prototype 01

Backpocket is a prototype you can try: an expense report that fills itself in from a photo of the receipt, highlights anything it isn't sure about, and checks every receipt against the expense policy.

Concept and design by [Victor Mascaro](https://victor-mascaro-ux.github.io/my-portfolio/), UX/AI designer.

**Live prototype:** https://victor-mascaro-ux.github.io/backpocket/

## The problem

Half of workers don't file expense reports for money they're owed, and the top complaint is the paperwork. Source: [WalkMe and Propeller Insights survey](https://ir.walkme.com/news-releases/news-release-details/walkme-survey-shows-half-workers-dont-file-expense-reports) of 2,400+ workers in the US, UK, Germany, Singapore and Australia, Nov 2023.

## How to try it

The bar above the phone walks you through 7 short tasks: scan Alex's 4 receipts and send the October report. Each task has a **Show me** button that does it for you, and if you pause for a few seconds, a pulsing ring on the phone points at the next tap. The app itself has no instructions in it, the same as a real product. Each receipt shows a different thing the AI does:

1. **Café**: everything is clear, so you just save it.
2. **Fuel**: the total is smudged. The AI shows the part of the photo it read and asks you to pick between the two readings.
3. **Client dinner**: the expense policy needs the names of the guests. The AI can't read them from a receipt, so it offers the names from your calendar event.
4. **Hotel**: the nightly rate is over the policy limit. The AI explains the limit and asks for a reason to send with the report.

## Design decisions

- **One photo fills it all in.** Snap the receipt and every detail is filled in for you.
- **Hard to read? It takes a guess.** Pick the right one, or type it in yourself.
- **The policy is built in.** Over a limit, or different from the receipt? Add a quick reason for your manager, right there.
- **Send whenever you like.** One receipt or all of them, the report is ready when you are.

## What's real

- The AI is scripted with 4 sample receipts, so it works the same for everyone.
- There's no backend, no analytics and no API key. Nothing you type leaves your browser.
- Backpocket, Acme, Alex Moreno (a sales rep), Jordan Lee (his manager, who approves the report), Sam Rivera (in finance), the merchants and the calendar event are all fictional.
- English and Brazilian Portuguese, picked from your browser language.

## Run it locally

Open `index.html` in a browser. It's a single static file with no build step.
