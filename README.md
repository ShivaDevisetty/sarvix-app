<p align="center">
  <img src="assets/sarvix-logo.png" alt="Sarvix Core logo: an orange stag's head" width="140">
</p>

<h1 align="center">Sarvix Core™</h1>

<p align="center"><b>Your whole world, one tap away.</b></p>

**One private app for your money and your health: spending, budgets, weight, body scans and health documents, on the web and on your phone. It's invite-only, it costs you nothing, and your files stay in your own Google Drive.**

![Invite only](https://img.shields.io/badge/access-invite_only-1B2533)
![Web and home screen](https://img.shields.io/badge/runs_on-web_%7C_home_screen-1B447A)
![Your Google Drive](https://img.shields.io/badge/your_files-your_Google_Drive-4285F4?logo=googledrive&logoColor=white)
![Costs](https://img.shields.io/badge/cost_to_you-%240-16a34a)
![No ads](https://img.shields.io/badge/ads_and_tracking-none-ff6a13)
![MIT licence for the text](https://img.shields.io/badge/text-MIT-555)
![Name and logo are trademarks](https://img.shields.io/badge/name_%26_logo-trademark%E2%84%A2-555)

[What it does](#what-it-does) · [Getting started](#getting-started) · [How to use](#how-to-use) · [Privacy](#privacy-and-security) · [FAQ](#faq) · [User guide](docs/user-guide.md)

---

## Contents

- [Why Sarvix Core](#why-sarvix-core)
- [The name](#the-name)
- [What it does](#what-it-does)
- [Getting started](#getting-started)
- [How to use](#how-to-use)
- [Use it on your phone](#use-it-on-your-phone)
- [Privacy and security](#privacy-and-security)
- [Limitations](#limitations)
- [FAQ](#faq)
- [Licence](#licence)

## Why Sarvix Core

Money and health usually live in two different apps, each with its own login, its own ads and its own idea of what your data is worth. Your health reports end up in one app's cloud, your receipts in another's, and your spending in a spreadsheet.

Sarvix Core puts them in one place, with simple rules: no ads, no tracking, no bank connections, no AI reading your records, and nothing to pay. The files you upload go into **your own** Google Drive, not someone else's server. This repository describes the app for the people who use it; its code isn't published here.

## The name

**Sarvix** is built from three parts:

| Element | Brand interpretation |
|---|---|
| **SAR** | Inspired by *Sarvam*, Sanskrit for all or everything |
| **V** | Vision, versatility, and connectivity |
| **IX** | Innovation, intelligence, and a futuristic identity |

## What it does

- **Spending.** Income, spending, net saved and savings rate for the month, where the money went by category and by merchant, and recurring payments. Drop a bank or card statement (CSV) on the page to import it: you review every row before anything is saved, and money out can only go into spending categories. **Scan receipt** reads a receipt photo on your own device to fill in an expense, and keeps nothing.
- **Budgets.** A monthly amount per category, with a bar that fills up as the month goes on.
- **Currencies.** US dollars, Indian rupees or both side by side, each amount in its own currency, or everything converted at the day's rate.
- **Fitness.** Weight, body fat and resting heart rate on one chart, with a 7-day average, where it's heading over the next weeks, and the target range you set. Weigh-ins that look off are marked and left out of the chart.
- **Health documents.** Body scans (DEXA), blood reports, diet periods (calories a day, from and to) and notes, together on one timeline. The files go to your own Google Drive.
- **Your account.** Change your password, connect or disconnect your Google Drive, and stay signed in on a phone, a tablet and a computer at once.
- **Help.** A Help button sends a question to the person who runs your Sarvix, and the reply comes back to the same place.
- **Everywhere.** A clean look in light or dark, with big clear headings, the same on a laptop and a phone.

## Getting started

1. **Get an invite.** Sarvix Core is invite-only: the person who runs your Sarvix sends you a sign-up link. Each link works once.
2. **Create your account** from that link: your name, your email and a password of at least 8 characters.
3. **Connect your Google Drive** under **Account › Personal Cloud Storage**. You need it before you can upload files; the app only ever sees the files it puts there.
4. **Start with Spending or Fitness.**

Every step is covered in more detail in the [user guide](docs/user-guide.md).

## How to use

### Track your money

1. In **Spending**, add expenses and income: pick the account it was paid from, a category and the currency.
2. To bring in a statement, drop the bank's CSV file at the top of the page. Map the columns, check each row's category, and add the rows you tick, all together or not at all. The file is read in your browser.
3. Set a **budget** per category and follow it through the month.
4. Use the currency switch in the page header for dollars, rupees or both.

### Look after yourself

1. In **Fitness**, log your weight (and body fat or resting heart rate if you have them).
2. The chart shows the trend for the last month, three months, year, or all of it, with diet periods shaded.
3. Upload a body scan or a blood report; it goes to your Google Drive and opens from its entry on the timeline.
4. Start a diet with its daily calories, and add notes for anything else worth remembering.

### Keep your account safe

1. Use a long password you don't use anywhere else, and keep it in a password manager: there's no reset link.
2. Changing your password under **Account › Password** signs you out on your other devices.
3. Check **Account › Personal Cloud Storage** to see which Google account your files go to.

## Use it on your phone

Open Sarvix Core on your phone and choose **Add to Home Screen** (Safari: the Share button; Chrome: the ⋮ menu). It then opens full-screen with its own stag icon, like an app. It needs an internet connection and a sign-in.

A phone app for Android, iPhone and the web is on the way. When it's ready, downloads will appear under **Releases** in this repository.

## Privacy and security

| What | Where it's kept | Who can see it |
|---|---|---|
| Your records (transactions, budgets, weigh-ins, notes) | The Sarvix database run by whoever runs your Sarvix | You, in the app. Other members never see them |
| Files you upload (health reports, documents, logos) | **Your own Google Drive**, in a `sarvam-maya-core` folder | You, and the app through Google's "files it created" permission |
| Your password | Stored only as a one-way hash | Nobody, not even the person who runs your Sarvix |
| Receipt photos | Nowhere: read on your device and thrown away | Nobody |

Sign-in is rate-limited (5 wrong passwords per email lock it for 15 minutes), sessions are secure cookies that last 30 days per device, and sign-up needs a one-time invite.

## Limitations

- **Invite-only.** You can't sign up on your own; ask the person who runs your Sarvix for an invite.
- **Spending and Fitness only.** Members have their own Spending, Fitness, Account and Help. Nothing is shared between accounts.
- **500 files per member.** Files in the Trash don't count. At the limit, uploads stop until you delete some.
- **No password reset by email.** If you forget your password, ask the person who runs your Sarvix for help.
- **Online only.** The home-screen app needs a connection; offline it shows a message, not your records.
- **Everything is entered by you.** There are no bank or fitness-tracker connections, on purpose.

## FAQ

**Does it cost anything?**
No. Your files use your own Google Drive's free storage, and the app itself costs you nothing.

**Where are my files, really?**
In your own Google Drive, in a folder called `sarvam-maya-core`. You can see them there, but leave them in place: the app keeps track of each file by its Drive id.

**What happens if I disconnect Google Drive?**
Your files stay in your Drive. The app can't open them until you connect the same Google account again, and you can't upload until you connect one.

**Can the person who runs my Sarvix read my password?**
No. Only a one-way hash of it is stored, so nobody can read it.

**Why does Google say the app isn't verified?**
Sarvix is a small private app, so Google shows that notice the first time you connect. It only asks for access to the files it creates itself.

**Where's the code?**
Not here. This repository is the public home of Sarvix Core for its users: what it does, how to use it, and downloads when they're ready.

## Licence

This repository contains no source code.

- **The text** (this README and the user guide) is under the [MIT licence](LICENSE).
- **The name and the logo are not.** **Sarvix™**, **Sarvix Core™** and the stag logo are trademarks, all rights reserved: you may mention the name to refer to the app, but not use the name or the logo for anything else without permission. See [TRADEMARKS.md](TRADEMARKS.md).
