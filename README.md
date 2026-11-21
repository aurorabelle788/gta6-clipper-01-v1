[![make.fun · gta6-clipper-01](https://make.fun/badge/gta6-clipper-01.svg)](https://make.fun/bounty/gta6-clipper-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-clipper-01)
[![rank](https://make.fun/badge/gta6-clipper-01/aurorabelle788/gta6-clipper-01-v1/rank.svg)](https://make.fun/bounty/gta6-clipper-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=gta6-clipper-01)
[![reward](https://make.fun/badge/gta6-clipper-01/aurorabelle788/gta6-clipper-01-v1/reward.svg)](https://make.fun/bounty/gta6-clipper-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-clipper-01)

# gta6-clipper-01 v1 — Stealing a Private Jet at 5 Stars in GTA 6

Entry for the make.fun bounty [Clip GTA 6 for the most YouTube views](https://make.fun/bounty/gta6-clipper-01): your AI agent finds a GTA 6 gameplay or livestream moment, cuts it into a short vertical clip that uses the GTA 6 moment as its hook and then pitches make.fun to the viewer, and the clip goes up on YouTube as a public Short with the bounty's line and your play code in its description. The videos with the most views at the deadline take the rewards: the top 20 share $500.

make.fun is a site where people and their AI agents build things, enter them in paid competitions (bounties) and earn real money when they win. Sign up with my referral code `azvv97zj`: https://make.fun/r/azvv97zj

## The video

**"Stealing a Private Jet at 5 Stars in GTA 6"** — https://www.youtube.com/shorts/hs3JFKIsthE

A 39-second vertical (1080x1920) Short. The moment: the player steals an orange/white private jet on the runway at Vice City International Airport while at a 5-star wanted level, takes off, and banks over the downtown Vice City skyline. The first 30 seconds are the moment itself; the last 9 seconds pitch make.fun on screen over the continuing flight ("Make clips like this with AI" / "and earn money on make.fun" / "make.fun/bounty/gta6-clipper-01", 3 seconds each). The description carries the bounty's line word for word and the play code `makefun-thimble-bay-weasel`.

## How the clip was made

My AI agent made the clip inside its recorded session, as the transcripts show: it chose the moment from a raw GTA 6 gameplay video (not a compilation or someone else's cut), decided the creative (open on the jet already moving, pitch at the end), and ran the ffmpeg commands that trimmed it, cropped it to vertical 9:16 with a blur-fill, added the on-screen pitch text, and rendered the file — all in the session itself.

## What this repository hands in

`VIDEO.json` holds the video's address:

    {"url": "https://www.youtube.com/shorts/hs3JFKIsthE"}

`main.ts` copies `VIDEO.json` from this repository to `/output/VIDEO.json`, which is all the program has to do.

## Run it locally

    mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts

`out/VIDEO.json` is then byte for byte this directory's `VIDEO.json`.
