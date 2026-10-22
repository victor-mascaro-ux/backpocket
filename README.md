# Backpocket · Prototype 01

Backpocket is a prototype you can try: an expense report that fills itself in from a photo of the receipt, highlights anything it isn't sure about, and shows how close you are to getting your money back.

Concept and design by [Victor Mascaro](https://victor-mascaro-ux.github.io/my-portfolio/), UX/AI designer.

**Live prototype:** https://victor-mascaro-ux.github.io/backpocket/

## The problem

Half of workers don't file expense reports for money they're owed, and the top complaint is the paperwork. Source: [WalkMe and Propeller Insights survey](https://ir.walkme.com/news-releases/news-release-details/walkme-survey-shows-half-workers-dont-file-expense-reports) of 2,400+ workers in the US, UK, Germany, Singapore and Australia, Nov 2023.

## How to try it

The bar above the phone walks you through 7 short tasks: scan Alex's 4 receipts and send the October report. Each task has a **Show me** button that does it for you, and a pulsing ring on the phone points at the next tap. The app itself has no instructions in it, the same as a real product. Each receipt shows a different thing the AI does:

1. **Café**: everything is clear, so you just save it.
2. **Fuel**: the total is smudged. The AI shows the part of the photo it read and asks you to pick between the two readings.
3. **Client dinner**: the expense policy needs the names of the guests. The AI can't read them from a receipt, so it offers the names from your calendar event.
4. **Hotel**: the nightly rate is over the policy limit. The AI explains the limit and asks for a reason to send with the report.

## Design decisions

- The AI fills in every field and highlights only what it isn't sure about, with the reason and the part of the photo it read.
- It knows the expense policy and asks only for what a photo can't tell it.
- The amount you'll get back grows with each receipt. Celebrations can be turned off in settings, and nothing is locked.
- Each receipt is one photo. You only type what the photo can't tell the AI.

## What's real

- The AI is scripted with 4 sample receipts, so it works the same for everyone.
- There's no backend, no analytics and no API key. Nothing you type leaves your browser.
- Backpocket, Acme, Alex Moreno (a sales rep), Jordan Lee (his manager, who approves the report), the merchants and the calendar event are all fictional.
- English and Brazilian Portuguese, picked from your browser language.

## Run it locally

Open `index.html` in a browser. It's a single static file with no build step.
