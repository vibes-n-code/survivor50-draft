# Survivor 50 Draft Tracker - Session Context

## Website
- Single file: `/Users/nick/Documents/AI/Projects/survivor50-draft/index.html`
- No backend — all data is embedded as JavaScript constants in the HTML file
- **Currently updated through Episode 8** (Apr 15, 2026)

## Machine Notes
- All personal projects now run on this computer (username: nick)
- Skill file: `/Users/nick/Documents/AI/Skills/survivor50-update-skill/SKILL.md`

---

## Current Cast Status (after Ep 8)

### Team Lizzy (purple)
| ID | Name | Status |
|----|------|--------|
| cirie | Cirie Fields | ALIVE — holds Extra Vote |
| ozzy | Ozzy Lusth | ALIVE — holds Boomerang Idol |
| chrissy | Chrissy Hofbeck | ELIMINATED Ep 8 (Voted Out, Double Duo twist) — jury #3 |
| angelina | Angelina Keeley | ELIMINATED Ep 5 (Voted Out) |
| colby | Colby Donaldson | ELIMINATED Ep 6 (Voted Out, Blood Moon) |
| jenna | Jenna Lewis | ELIMINATED Ep 1 (Voted Out) |

### Team Tanner (blue)
| ID | Name | Status |
|----|------|--------|
| aubry | Aubry Bracco | ALIVE (idol used Ep 7) |
| joe | Joe Hunter | ALIVE |
| ricky | Rick Devens | ALIVE |
| coach | Coach Wade | ELIMINATED Ep 8 (Voted Out, Double Duo twist) — jury #2 |
| stephanie | Stephenie LaGrossa | ALIVE — holds Steal-a-Vote |
| savannah | Savannah Louie | ELIMINATED Ep 2 (Voted Out) |

### Team Nick (green)
| ID | Name | Status |
|----|------|--------|
| dee | Dee Valladares | ELIMINATED Ep 7 (Voted Out) — jury #1 |
| jonathan | Jonathan Young | ALIVE |
| rizo | Rizo Velovic | ALIVE — holds Boomerang Idol |
| q | Q Burdette | ELIMINATED Ep 3 (Voted Out) |
| genevieve | Genevieve Mushaluk | ELIMINATED Ep 6 (Voted Out, Blood Moon) |
| kyle | Kyle Fraser | ELIMINATED Ep 1 (Medical Evacuation) |

### Team Casey (orange)
| ID | Name | Status |
|----|------|--------|
| christian | Christian Hubicki | ALIVE |
| charlie | Charlie Davis | ELIMINATED Ep 5 (Voted Out) |
| mike | Mike White | ELIMINATED Ep 4 (Voted Out) |
| emily | Emily Flippen | ALIVE |
| kamilla | Kamila Karthigesu | ELIMINATED Ep 6 (Voted Out, Blood Moon) |
| tiff | Tiffany Ervin | ALIVE |

---

## Active Advantages (after Ep 8)
| ID | Name | Holder | Status | Notes |
|----|------|--------|--------|-------|
| boomerang-idol-ozzy | Billie Eilish Boomerang Idol | ozzy | active | Boomerang clause void (Genevieve eliminated) |
| boomerang-idol-genevieve | Billie Eilish Boomerang Idol | rizo | active | Found by Genevieve, gifted to Rizo (Ep 4) |
| extra-vote-cirie | Extra Vote | cirie | active | Q→Ozzy→Cirie chain |
| steal-a-vote-stephanie | Steal-a-Vote | stephanie | active | Won on journey in Ep 7 |
| boomerang-idol-aubry | Billie Eilish Boomerang Idol | aubry | used | Played Ep 7, negated 0 votes |

---

## Jury (in order)
1. Dee Valladares (Ep 7)
2. Coach Wade (Ep 8)
3. Chrissy Hofbeck (Ep 8)

---

## Recommended Next Steps for New Session
1. Research Episode 9 (airs Apr 22, 2026) recap after it airs
2. Check for DK Network power rankings ~2 days after (URL pattern: dknetwork.draftkings.com/2026/04/{DD}/survivor-50-power-rankings-fallout-after-episode-9/)
3. Update EPISODES, ADVANTAGES, odds, and POWER_RANKINGS (now uses ep8Rank field for movement arrows)
4. Push to GitHub Pages (see SKILL.md for git commands with vibes-n-code token)

## Render Code Note
- Power rankings movement arrows now use `ep7Rank` field (updated in Ep 8 session)
- Render code: `entry.ep7Rank || entry.ep6Rank || entry.ep3Rank` (backward compatible)
- Next update should use `ep8Rank` field in rankings entries and update render code line accordingly
