# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users
Primary: owners and QC leads of dubbing studios that deliver dubbed series and films to streaming and broadcast clients, internationally. Their situation: a dubbed episode must pass the client's delivery QC; a failed QC means a redo, a late delivery and a client who trusts the studio less. Their job: catch what the client's QC would flag before the episode leaves the studio.
Secondary: the dub mixers who use the app in their session (Pro Tools, Logic, Nuendo, Cubase) and step through the markers.

## Product Purpose
Dubbing QC is a Mac app that compares a dubbed dialogue stem with the original-version (OV) dialogue stem and lists the places a mixer should listen to: missing lines and efforts (breaths, laughs, reactions), laughs and walla the dub dropped, extra sounds, reverb and pan that differ from the OV, sync shifts, cut-off line ends, clicks, clipping, EQ/voice-treatment mismatches, LFE problems, file naming, OV audio left in the dub, printmaster sync and loudness. Output: DAW markers plus a PDF report. Success: a studio runs it on every episode before delivery and stops failing client QC on things a machine can find.

## Positioning
It compares the dub against the original, channel by channel, rather than checking the dub alone against loudness specs. Every threshold was measured against real delivery-QC reports, planted defects and listening tests, not guessed. It runs entirely on the Mac: no audio, report or file name leaves it. Findings are candidates to listen to, not verdicts.

## Operating Context
A studio receives OV stems and records/mixes the dub; before delivery the QC lead or mixer drops the OV and dub folders (split-mono 5.1 WAV) on the app, runs a check (about a minute per 55-minute episode), imports the markers into the DAW session and listens. Season mode runs a folder of episodes in one go. Clients' delivery QC reports grade issues as Blocker / Major.

## Capabilities and Constraints
- Mac app, macOS 14 or later, Apple Silicon and Intel, notarised Developer ID download (`Dubbing-QC.dmg` from GitHub Releases).
- Licence required to run checks. Free 3-day trial, once per person and per Mac. Rentals: €49 / 10 days, €89 / 30 days, €159 / 60 days; €399 for one year (one payment, no automatic renewal). Prices exclude VAT. Sold on redpixl.dev (RedPixl s.r.o.).
- Works offline after activation. Optional on-device speech recognition (off by default).
- Primary action on the site: download the app and start the free 3-day trial.
- Known limits exist and are documented in the manual; never claim it replaces a human QC pass.

## Brand Commitments
- Name: Dubbing QC. Maker: RedPixl s.r.o.
- The green app icon and green as the brand colour stay (icon assets in the repo root: `icon.png`, `icon-512.png`).
- The real app screenshots stay as the main imagery (`shot-*.png`, `extra-screenshots/`), all native 2x captures of 1.0.1 with neutral demo names.
- Voice: plain, precise, studio-professional; no hype.

## Evidence on Hand
- Tested on a real 55-minute TV episode that also had a professional delivery-QC report: the app flagged all 5 reverb and pan issues in that report, and found 11 more real reverb and pan differences the human QC pass had missed, each confirmed by listening. May be stated publicly, anonymised: no client, broadcaster or show name.
- Thresholds measured against real QC reports, planted-defect tests and listening tests.
- Pro Tools marker import confirmed by a partner sound engineer; Nuendo/Cubase CSV follows the documented format but is not yet confirmed in a real session.
- Sample PDF report: `Dubbing-QC-Sample-Report.pdf`. Manual: `manual.html` + `DubbingQC-Manual.pdf`.
- No customer testimonials, logos or usage numbers exist; do not invent any.

## Product Principles
1. Prefer recall: better a false positive than a missed problem.
2. A finding is a place to listen, never a verdict.
3. Nothing leaves the Mac.
4. Measure, don't guess: every limit traces to real evidence.
5. Fit the studio's own workflow (its DAW, its session timecode), don't replace it.
