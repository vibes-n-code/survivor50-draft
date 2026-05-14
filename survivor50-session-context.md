# Survivor 50 Draft Tracker - Session Context

## Website
- Single file: `/Users/nick/Projects/survivor50-draft/index.html` (also reachable via `/Users/nick/Workspace/Projects/survivor50-draft/index.html`)
- No backend — all data is embedded as JavaScript constants in the HTML file
- **Currently updated through Episode 12** (May 13, 2026)
- Power rankings stamped at EP11 (DK rankings published May 7, 2026); EP12 rankings would arrive Friday May 15
- Finale airs Wednesday May 20, 2026

## Machine Notes
- All personal projects now run on this computer (username: nick)
- Skill file: `/Users/nick/Workspace/AI-Operations/Skills/survivor50-update/SKILL.md`

---

## Current Cast Status (after Ep 12 — Final 5)

### Team Lizzy (purple)
| ID | Name | Status |
|----|------|--------|
| cirie | Cirie Fields | ELIMINATED Ep 12 (Voted Out 4-2) — jury #9 |
| ozzy | Ozzy Lusth | ELIMINATED Ep 11 (Voted Out 4-1, split tribal) — jury #7 |
| chrissy | Chrissy Hofbeck | ELIMINATED Ep 8 (Voted Out, Double Duo twist) — jury #3 |
| angelina | Angelina Keeley | ELIMINATED Ep 5 (Voted Out) |
| colby | Colby Donaldson | ELIMINATED Ep 6 (Voted Out, Blood Moon) |
| jenna | Jenna Lewis | ELIMINATED Ep 1 (Voted Out) |

### Team Tanner (blue)
| ID | Name | Status |
|----|------|--------|
| aubry | Aubry Bracco | ALIVE — Final 5 |
| joe | Joe Hunter | ALIVE — Final 5 (won EP12 day-22 immunity) |
| ricky | Rick Devens | ELIMINATED Ep 12 (Voted Out 6-0, Shot in the Dark failed) — jury #8 |
| coach | Coach Wade | ELIMINATED Ep 8 (Voted Out, Double Duo twist) — jury #2 |
| stephanie | Stephenie LaGrossa | ELIMINATED Ep 10 (Voted Out 8-2) — jury #5 |
| savannah | Savannah Louie | ELIMINATED Ep 2 (Voted Out) |

### Team Nick (green)
| ID | Name | Status |
|----|------|--------|
| dee | Dee Valladares | ELIMINATED Ep 7 (Voted Out) — jury #1 |
| jonathan | Jonathan Young | ALIVE — Final 5 (orchestrated EP11 Ozzy blindside) |
| rizo | Rizo Velovic | ALIVE — Final 5 — holds Boomerang Idol (kept in pocket through EP12) |
| q | Q Burdette | ELIMINATED Ep 3 (Voted Out) |
| genevieve | Genevieve Mushaluk | ELIMINATED Ep 6 (Voted Out, Blood Moon) |
| kyle | Kyle Fraser | ELIMINATED Ep 1 (Medical Evacuation) |

### Team Casey (orange)
| ID | Name | Status |
|----|------|--------|
| christian | Christian Hubicki | ELIMINATED Ep 9 (Voted Out 6-3-2, forced self-vote) — jury #4 |
| charlie | Charlie Davis | ELIMINATED Ep 5 (Voted Out) |
| mike | Mike White | ELIMINATED Ep 4 (Voted Out) |
| emily | Emily Flippen | ELIMINATED Ep 11 (Voted Out 2-1 on revote) — jury #6 |
| kamilla | Kamila Karthigesu | ELIMINATED Ep 6 (Voted Out, Blood Moon) |
| tiff | Tiffany Ervin | ALIVE — Final 5 (won EP12 day-23 immunity, 'Inconceivable' puzzle) |

---

## Active Advantages (after Ep 12)
| ID | Name | Holder | Status | Notes |
|----|------|--------|--------|-------|
| boomerang-idol-genevieve | Billie Eilish Boomerang Idol | rizo | active | Still in Rizo's pocket entering finale; boomerang clause void (Genevieve eliminated Ep6) |
| boomerang-idol-ozzy | Billie Eilish Boomerang Idol | ozzy | eliminated | Exited the game in Ozzy's pocket Ep11 |
| extra-vote-cirie | Extra Vote | cirie | used | Played Ep11 tribal #1 to force 2-2-2 tie / flush Rick's idol |
| super-beware-idol-rick | Super Beware Advantage Idol | ricky | used | Played on himself Ep11 tribal #1; Rick voted out Ep12 without protection |
| steal-a-vote-stephanie | Steal-a-Vote | stephanie | used | Played Ep 10 on Rick (already immune); no impact |
| boomerang-idol-aubry | Billie Eilish Boomerang Idol | aubry | used | Played Ep 7, negated 0 votes |

---

## Jury (in order — 9 members heading into finale)
1. Dee Valladares (Ep 7)
2. Coach Wade (Ep 8)
3. Chrissy Hofbeck (Ep 8)
4. Christian Hubicki (Ep 9)
5. Stephenie LaGrossa (Ep 10)
6. Emily Flippen (Ep 11)
7. Ozzy Lusth (Ep 11)
8. Rick Devens (Ep 12)
9. Cirie Fields (Ep 12)

---

## Final 5 (entering May 20 finale)
- Aubry Bracco (Tanner)
- Joe Hunter (Tanner)
- Jonathan Young (Nick)
- Rizo Velovic (Nick) — last idol in play
- Tiffany Ervin (Casey)

Finale airs live Wednesday May 20, 2026 at 8pm ET on CBS / Paramount+ — $2M prize (doubled via Rick's MrBeast coin-flip in EP10).

---

## Render Code Note
- Power rankings movement arrows now use `ep9Rank` field (updated in EP11 session, skipping the never-pulled EP10 rankings)
- Render code: `entry.ep9Rank || entry.ep8Rank || entry.ep7Rank || entry.ep6Rank || entry.ep3Rank` (backward compatible)
- Next update (after finale) should use `ep11Rank` if DK publishes a finale-eve ranking
