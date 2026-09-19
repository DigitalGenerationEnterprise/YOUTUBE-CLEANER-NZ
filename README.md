# YOUTUBE-CLEANER-NZ
Youtube has been taken over by sparmer and CEO of google is part of problem

# YouTube Search Has Forgotten What Search Is For

YouTube has become one of the biggest stores of human knowledge ever built. It is also becoming harder to find the thing you actually asked for.

Search for a local issue, a repair guide, a product review or a piece of news and the pattern is familiar. The results drift. Shorts interrupt the page. The same clip appears under several titles. Reuploads outrank original sources. Thumbnails shout. Titles promise a revelation and deliver ten minutes of filler. A query with obvious New Zealand intent can still return a wall of material with weak or no local connection.

This is not a complaint about people from somewhere else. It is a complaint about relevance.

The platform is doing what its incentives reward. A useful answer can end a session. A provocative answer can start a chain of clicks. Repetition is cheap, sensational packaging works, and global inventory is easier to serve than careful local context. When the system is trained to maximise attention, search quality becomes one input among many rather than the main job.

That difference matters. Search is a promise: I will use the words you gave me to help you find the best answer. A recommendation feed makes a different promise: I will keep showing you things you may watch. YouTube increasingly blends the two, and users pay the cost in time.

## Local intent is real intent

If I search for Auckland transport, New Zealand housing, Wellington weather or an NZ product supplier, location is not a decorative keyword. It changes the answer.

Rules, prices, organisations, vocabulary and public services differ by country. A technically good result can still be practically useless if it belongs to the wrong place. Yet most platforms give users weak locality controls. We can add more words, use quotes and block a channel after the damage is done, but we cannot easily say: for this kind of query, prefer these sources, recognise these local signals, suppress these formats and explain why a result was moved.

That should be normal.

## The answer is not another secret algorithm

The tempting response to a bad ranking system is a better ranking system. That helps, but it leaves the same basic problem: somebody else decides what “better” means and the user sees the result, not the rule.

A more durable answer is transparent, user-controlled filtering.

Let me choose preferred channels. Let me block channels I have already judged to be low value. Let me suppress Shorts when I am doing research. Let me collapse likely repeats. Let me apply narrow clickbait rules and turn them off when they get in the way. When my own query has local intent, let me require some visible local signal. Most importantly, tell me why something was boosted or hidden.

That last part changes the relationship. A black box asks for trust. An explainable rule asks for judgment.

## Small tools can restore agency

That is the thinking behind the NZ YouTube Relevance Cleaner, a small browser extension I have been developing for my own use.

It does not try to identify where a creator “really” comes from. It does not infer ethnicity or nationality. It works with visible text signals, the query I entered, and lists I control. It can boost NZ terms and preferred channels, hide manually blocked channels, suppress Shorts, flag likely duplicate titles, apply a short list of transparent clickbait patterns and show the reason for each decision.

Everything runs in the browser. There is no analytics service, no remote code and no external collection of browsing data. The source is inspectable because trust should come from what a tool does, not what its author claims.

This is not a claim that a handful of rules can solve discovery. Heuristics make mistakes. YouTube changes its page structure. Text is only a signal, not proof. But user-controlled mistakes are easier to inspect, switch off and improve than invisible platform decisions.

## What platforms should learn

The larger opportunity is not “more filtering”. It is better control.

Platforms could give users named search modes: local, original sources, long-form, recent, technical, low-repetition. They could expose why a result was shown. They could let people save source preferences by topic. They could detect and group reuploads without erasing legitimate commentary. They could separate search from recommendation more honestly.

None of this requires targeting protected groups. It requires taking intent seriously.

Users are not asking for a perfectly sanitised internet. We are asking for tools that respect the question, make trade-offs visible and let us correct the system when it gets them wrong.

YouTube search will improve when relevance is treated as a user right rather than a side effect of engagement. Until then, small transparent tools can give some control back to the person doing the searching.

None selected 


Skip to content
Using Gmail with screen readers
Conversations
me
Article hero image + revised GitHub README - NZ YouTube Relevance Cleaner
Three attachments for the YouTube work: - youtube-used-to-answer-hero.png - hero image for "YouTube Used to Answer. Now It Wants Your Evening." Editorial style, New Zealand-local (Southern
 
22:12
Article hero image + revised GitHub README - NZ YouTube Relevance Cleaner
Inbox

Anthony Blomfield <kiwianthony@gmail.com>
Attachments
22:12 (10 minutes ago)
to me

Three attachments for the YouTube work:

- youtube-used-to-answer-hero.png - hero image for "YouTube Used to Answer. Now It Wants Your Evening." Editorial style, New Zealand-local (Southern Cross, Auckland skyline silhouette, silver fern): a wall of noisy search clutter resolving into a short, useful local list. No logos, no baked-in text, so a headline can sit over it.
- README.md - revised user-focused GitHub README for the NZ YouTube Relevance Cleaner: the problem, what it does, who it is for, install on Kubuntu (Chrome/Chromium), first-run setup, controls, privacy, limitations, troubleshooting, removal, screenshots and contributing.
- readme-preview.html - the README rendered as it will look on GitHub, for a quick read-through.

Repo placement: the README expects the hero at assets/hero.png; the settings screenshot stays at assets/screenshots/settings.png. The article body is unchanged.

Instinct
 3 attachment
  •  Scanned by Gmail
README.md
100%
# NZ YouTube Relevance Cleaner

![Filtering a wall of noisy results into a short, useful local list](assets/hero.png)

**Cleaner YouTube search for New Zealanders.** A small, inspectable browser extension that boosts local and preferred results, hides channels you have already written off, suppresses Shorts, duplicates and clickbait, and shows the reason for every decision. No tracking, no account, no external service.

## The problem

You search YouTube for something with obvious local intent - an Auckland repair guide, NZ news, a Kiwi product review - and the results drift. Shorts interrupt the page. The same clip appears under several titles. Reuploads outrank the original. Thumbnails shout. A query that clearly means New Zealand still returns a wall of material with no local connection. The platform is optimizing for watch time, not for your question.

## What it does

Runs a small set of transparent rules on YouTube search and result pages, entirely in your browser:

- **Boosts NZ and local signals** - a configurable list of terms such as `new zealand`, `aotearoa` and major centres
- **Boosts your preferred channels** so sources you trust surface first
- **Hides channels on your own block list**
- **Suppresses Shorts** when you want answers, not a feed
- **Hides likely duplicates** - the same normalized title already visible on the page
- **Filters narrow, declared clickbait patterns** - mostly-capital titles, `!!!` punctuation, heavy emoji, and a short public list of bait phrases
- **Optional local-intent mode** - when your query itself has New Zealand intent, require a visible NZ signal (off by default)
- **Shows the reason** for every boost or hide, right on the result

Every rule can be switched off. Preferred channels override every hide rule, including your own block list. The extension never decides who a creator is: it reads visible text, your query and your lists. It does not infer or filter anyone's nationality, ethnicity or other protected traits.

## Who it is for

- People in New Zealand whose searches carry local intent and whose results ignore it
- Researchers, students and tradespeople tired of wading through reuploads and Shorts to find one useful video
- Viewers who want Kiwi channels and original sources to outrank copy uploads
- Anyone who prefers ranking rules they can read, switch and override over another black box

It is a relevance tool, not a gatekeeper. If a rule ever gets in your way, turn that rule off and keep the rest.

## Screenshots

![Settings screen: core controls, quality rules, channel lists and local signals](assets/screenshots/settings.png)

## Install on Kubuntu (Chrome or Chromium)

1. Download the release archive and verify its checksum.
2. Extract it to a permanent folder, such as `~/Applications/nz-youtube-cleaner`.
3. Open `chrome://extensions`.
4. Turn on **Developer mode**.
5. Click **Load unpacked**.
6. Select the extracted folder containing `manifest.json`.
7. Pin the extension, then refresh any open YouTube tabs.

Keep the extracted folder in place. Chromium loads the extension from that folder every time it starts.

## First-run setup

1. Click the extension icon in the toolbar. The popup holds the four everyday switches: **Enabled**, **Boost NZ results**, **Suppress Shorts** and **Show reasons**. Popup changes save instantly.
2. Click **Open all settings** to make it yours:
   - add channels you trust to **Preferred channels** (one per line)
   - add channels you never want to see again to **Blocked channels**
   - edit the **NZ and local signals** list to suit your region
   - decide how strict the quality rules should be
3. Click **Save settings**, reload YouTube and run a search.
4. Keep **Show reasons** on while you tune. Every moved result says why, so you can judge the rules instead of trusting them.

The defaults are a sensible middle: NZ boost, Shorts suppression, duplicate and clickbait filters, block-list hiding and reason labels are on; the strict local-intent requirement is off until you ask for it.

## Controls

Popup (quick switches):

| Switch | What it does | Default |
| --- | --- | --- |
| Enabled | Applies all rules on YouTube | On |
| Boost NZ results | Boosts results matching your NZ/local terms | On |
| Suppress Shorts | Hides Shorts from results | On |
| Show reasons | Labels each boosted or hidden result with the rule that fired | On |

Full settings page (**Open all settings** in the popup):

| Setting | What it does | Default |
| --- | --- | --- |
| Filter duplicates | Hides repeated normalized titles on the current page | On |
| Filter clickbait | Applies the declared caps, punctuation, emoji and bait-phrase rules | On |
| Hide blocked channels | Hides channels on your block list | On |
| Require NZ signal for local searches | Hides results with no NZ signal when your query has local intent | Off |
| Preferred channels | Always shown and boosted; overrides every hide rule | Empty |
| Blocked channels | Hidden while **Hide blocked channels** is on | Empty |
| NZ and local signals | The term list used for boosting and local intent | Preloaded NZ list |

Changes on the settings page apply after **Save settings**. **Restore defaults** returns everything to the state above.

## Privacy

The extension requests only two permissions:

- `storage`, to save your settings (synced by Chromium between your own browsers)
- `https://www.youtube.com/*`, to apply rules on YouTube pages

There is no background worker, remote code, telemetry, analytics, account access, browsing-history permission or extension-operated network service. Your channel lists and settings never leave your browser's own sync storage. See [PRIVACY.md](PRIVACY.md) and [SECURITY.md](SECURITY.md).

## Limitations

- YouTube changes its HTML often, so selectors may need maintenance.
- Text signals are hints, not proof of location.
- CSS boosting cannot fully reorder every YouTube shelf.
- Heuristics can produce false positives. Switches and preferred channels provide overrides.
- The extension does not inspect speech, images, geolocation, uploader identity or private account data.
- Unpacked installs do not auto-update.

## Troubleshooting

- **Installed, but nothing changes on YouTube.** Refresh the tab. Rules apply when a page loads, so tabs opened before install need a reload.
- **The extension vanished after a reboot.** Chromium loads unpacked extensions from the extracted folder. If the folder was moved or deleted, restore it and use **Load unpacked** again.
- **Too much is being hidden.** Turn off the clickbait or duplicate filters, or add the affected channel to **Preferred channels**.
- **A channel I like keeps disappearing.** Add it to **Preferred channels**. Preferred overrides every hide rule, including the block list.
- **No reason labels on results.** Enable **Show reasons** in the popup.
- **Settings did not stick.** Popup switches save instantly, but the full settings page only applies changes when you click **Save settings**.
- **Rules stopped working after a YouTube update.** YouTube rewrites its page structure regularly. File an issue with the page type, browser version and a redacted screenshot.

## Remove it

1. Open `chrome://extensions`.
2. Find **NZ YouTube Relevance Cleaner** and click **Remove**.
3. Delete the extracted folder.

Removing the extension deletes its stored settings. Nothing else is left behind: no account, no server, no background process.

## Test and inspect

Requirements: Node.js and Python 3.

```bash
node tests/rules.test.js
python3 tests/static_check.py
```

The main behavior is in `src/rules.js` and `src/content.js`. The manifest and all UI code are plain text and included in the repository.

## Contributing

Bug reports should include the YouTube page type, browser version, expected result, actual result and a redacted screenshot if useful. Do not include private viewing data. Read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a change.

## Release and license

See [CHANGELOG.md](CHANGELOG.md). The recommended repository description and topics are in [docs/GITHUB.md](docs/GITHUB.md). Licensed under the MIT License - see [LICENSE](LICENSE).
Displaying README.md.
