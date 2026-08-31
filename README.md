# MTL Volunteering — site

The cross-sport volunteer guide for the **Mountain Top League** (West Orange, NJ), live at **<https://volunteering.mountaintopleague.com/>**. It's a plain, file-based Jekyll site — every page is a simple text file you (or your AI agent) can edit. No logins to a website builder, no waiting on anyone else.

> **The easiest way to change anything: just ask your agent.**
> *"Add the AED location at O'Connor Park."* · *"Update the team-bag pickup window."* · *"Document how field gear gets set up at Stagg."*
> Then look over the PR it opens — every PR automatically gets a **preview site link and a visual diff** so you can see exactly what changes before it goes live.

Several sections are marked **"Coordinator input needed"** — they're the point of this site. If you know how something actually works, that knowledge belongs here instead of in word of mouth.

## How the site is laid out

| You want to change… | Edit this file |
|---|---|
| Home page & per-sport contacts | `index.md` |
| League House (access, team bags, supplies) | `league-house.md` |
| Gear (ordering, distribution, field gear) | `gear.md` |
| Sportsmanship & balanced teams | `sportsmanship.md` |
| Safety (first aid, concussions, training) | `safety.md` |
| Menu | `_data/nav.yml` |
| The colors and look | `_sass/_base.scss` |
| Site title / description | `_config.yml` |

## Previewing and publishing

- **Every PR gets a live preview**: a comment appears on the PR with a link to a full preview of the changed site, plus a visual diff against the current site. Review those, then merge — the live site updates within a couple of minutes.
- **Local preview** (optional): `bundle install` once, then `bundle exec jekyll serve` and open <http://localhost:4000/>.

## The bigger picture

This is the cross-sport companion to the Mountain Top League's per-sport sites — [mtl-soccer](https://github.com/SiliconSaga/mtl-soccer) ([soccer.mountaintopleague.com](https://soccer.mountaintopleague.com/)) and [mtl-hockey](https://github.com/SiliconSaga/mtl-hockey) ([hockey.mountaintopleague.com](https://hockey.mountaintopleague.com/)); the [Mountain Top League site](https://mountaintopleague.com/) remains the league-wide primer. CI (deploy + PR preview + visual diff) is shared via [volundr](https://github.com/SiliconSaga/volundr).
