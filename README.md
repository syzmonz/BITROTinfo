# BITROT — Info and FAQ page contents

Written for the beta, assuming this checklist is done: universal API key instead of rigs, 10,000 daily Hold per player, Zigbee/LoRa, Wax and Echo hidden, natural Blight, no fast-forward.

---

# Info: How BITROT works

## The short version

BITROT is a territory game played by wardriving. Go out with a compatible rig, record the Wi-Fi and Bluetooth around you, and upload the log. Every network you heard claims a little ground on the map for your team.

Then the ground starts to rot. Territory you don't keep scanning fades, turns ghost and goes back up for grabs. Rival teams scanning the same streets drain your hold on them. Towns have councils, councils have politics, and politics end in towns falling.

You never connect to anything. BITROT only uses what devices already broadcast to everyone nearby.

## The map

The world is split into hexagonal **tiles**, each about 350 m across. A tile nobody has scanned is **undiscovered**. The first team to scan it is its **pioneer**, and that stays in the tile's history forever.

Every team holds a number between 0 and 100 on each tile, called **Hold**. The team with the most Hold **owns** the tile and it shows in their colour and pattern. On a tie, the current owner keeps it.

When the last team's Hold on a tile reaches 0, the tile becomes a **ghost**. Ghosts belong to nobody, speed up rot on the tiles around them, and give a bonus to whoever reclaims them.

## Scanning and Hold

- Each network you upload adds **2 Hold** to the tile it was heard in.
- A network counts for a quarter until someone from a different team hears it too. This stops people inventing networks.
- The same network only counts once per team every 24 hours, so driving the same road twice in a day does nothing extra.
- A tile can gain at most **40 Hold per team per day**, and you can add at most **10,000 Hold a day** in total. Busy city streets fill up fast; this keeps the countryside worth visiting.
- Scans have to be recent. Anything recorded more than **72 hours** before you upload it is ignored.

## Takeovers

When you scan a tile another team holds, your gain drains their Hold. Raid it hard enough and it becomes yours. How much you drain depends on your team type, theirs, the month's condition and the tile itself (fortress tiles, for example, are hard to take). Brand-new teams are drained at half strength for their first week, or until they make their first takeover.

## Rot

Every tile loses Hold every hour. A full tile left alone fades to nothing in about five days, but lots of things change the speed:

| Speeds it up | Slows it down |
| --- | --- |
| Summer (×1.5) | Winter (×0.5) |
| Transit areas | Suburbs and wilds |
| Ghost tiles next door (+25% each) | Being connected to your home territory |
| Blight on or next to the tile (×2) | A Granary in the town |
| Being cut off from your home territory | A council voting rot to Slow |
| Some monthly conditions and team types | Freezes and Salt stop it entirely |

However the factors stack, rot never runs faster than ×3.

**Supply lines.** Your team's biggest connected block of tiles is its home territory. Tiles joined to it rot slower; isolated pockets rot faster. Leave a gap and the far side starts dying.

The tile panel shows every factor affecting a tile, and how long it has before it turns ghost.

## Blight

Blight is a creeping rot. Tiles in or next to it rot twice as fast, and it spreads one ring further every day. It now and then appears on its own where a team has piled a lot of Hold into a city. To clear a Blight tile, scans from two different teams have to land on it within 24 hours, or someone uses an Antidote.

## Teams

You play as part of a team of up to 15. Hold belongs to the team, not to you. When you create a team you pick its type, and the captain can change it once per season.

| Type | Rot | Takeovers | Defence | Special |
| --- | --- | --- | --- | --- |
| Wardens | Slower (×0.8) | Slightly stronger (×1.05) | Weaker (drained ×1.25) | |
| Raiders | Faster (×1.25) | Stronger (×1.5) | Normal | |
| Anarchists | Fastest (×1.5) | Strongest (×1.75) | Weaker (drained ×1.25) | Never sit on a council, stir up double Unrest, don't suffer the extra rot in fallen towns |
| Cartographers | Normal | Normal | Normal | +50% Hold on tiles nobody had found |
| Scavengers | Normal | Normal | Normal | +50% Hold reclaiming ghost tiles |

Captains can invite, kick, hand over the captaincy and disband the team.

## Towns and councils

Every town and city has a **council outpost**. Your team's **stake** in a town is the Hold it owns there compared with everything the town could hold. The biggest stakeholders take the seats:

| Size | Seats |
| --- | --- |
| Village (under 10,000 people) | 3 |
| Town (under 100,000) | 5 |
| City | 7 |
| Capital | 9 |

A seat needs at least 5% of the stake. Bigger stake means a bigger vote.

**Monthly vote.** Seated teams vote before the 1st of each month on:
- **Rot level**: Slow (half rot, but tiles there score less), Normal, or Fast (more rot, more score)
- **Town Law**:
  - **Sanctuary**: takeovers drain 40% less
  - **Toll**: teams without a seat gain 25% less Hold
  - **Bounty**: bonus points for taking tiles from a named team
  - **Embargo**: a named team can't use items in the town
  - **Open Market**: seated teams earn 50% more materials there

Your team's vote is its members' majority. A seated team that doesn't vote at all raises Unrest.

**Treasury and buildings.** A share of the materials seated teams earn in a town goes into its treasury, and members can donate more. Councils vote to spend it on buildings that last 30 days and can be repaired before they crumble:
- **Watchtower**: shows takeovers around the outpost and reveals Shrouded rivals
- **Walls**: takeovers around the outpost drain half
- **Granary**: the whole town rots 20% slower

**Politics.** Councils can pass a no-confidence motion to bar a seated team for 30 days, which needs three-quarters of the other seats. Rewards shrink if you spread too thin: your team's best 3 seats pay in full, the next 3 pay half, and beyond that seats only give you a vote.

## Unrest and fallen towns

Every town has **Unrest** from 0 to 100. It rises when teams without a seat scan around the outpost, when seated teams skip votes, and when someone secretly undermines the council. It falls when seated teams patrol the outpost and over time. At 100 the council **falls**.

A **fallen** town has no laws, rots faster, and is ruled by a **Warlord**: the team with the biggest stake, re-checked weekly. The Warlord can issue one decree per week (Bounty or Toll). There are two ways back:
- **Reform**: the Warlord's captain calls a congress, and a week later the council returns with the reformers holding a guaranteed seat.
- **Restoration**: three or more teams holding over half the town patrol the outpost on 5 days within a week.

## Free Cities

A fallen town that nobody restores within 30 days becomes a **Free City** for 90 days, then gets a council again. Some towns are Free Cities from the start and stay that way for good.

In a Free City there are no takeovers and no Unrest, and Hold gained there doesn't count towards the leaderboard (discoveries still do). Free Cities are where teams trade: anyone who's scanned there in the last week can post or take offers of materials and items.

## Materials, items and the shop

Some networks give crafting materials as well as Hold. You get one unit for every 5 networks of a kind:
- **Static**: 5 GHz and 6 GHz Wi-Fi
- **Iron**: WPA3 and enterprise Wi-Fi
- **Spores**: Bluetooth LE devices

You can craft items from materials, or your team can buy them with shop points earned from its monthly leaderboard finish. Each item has a monthly buying limit. **Items only work where you are**: to fire one you upload a short scan, under 15 minutes old, that hears at least 3 networks already known in that tile or town.

| Item | What it does |
| --- | --- |
| Pulse | Drains 40% of rival Hold on the tile and 15% on the six around it. Not in Free Cities |
| Beacon | A ghost or empty tile starts at 30 Hold for your team |
| Overclock | Your scans add double Hold for an hour |
| Shroud | Rivals see your tiles in a town as undiscovered for 24h, until one of them scans there |
| Audit | Exposes a team that undermined your council in the last week and bars it for 30 days |

More items arrive as new materials are added.

## Freezes

Going on holiday? Freezes stop rot completely:
- **Personal freeze**: 14 days per season, used 3 to 14 days at a time. It covers the tiles where you supplied most of your team's Hold.
- **Team freeze**: once per season, up to 7 days, if most of the team votes for it.

Both start 12 hours after you set them, so they can't be used to dodge an attack already under way.

## Monthly conditions

Each month has a condition picked from how the game went the month before, announced a week ahead with the reason:

| Condition | Effect |
| --- | --- |
| Clear | Nothing special |
| Damp | Rot 50% faster |
| Dry Spell | Rot at half speed |
| Hard Frost | No rot for the first week |
| Open Season | Takeovers drain 50% more |
| Static Storm | 5 GHz networks give double Hold |
| Bluetide | Bluetooth LE devices give Hold, not just Spores |
| Gold Rush | Rural tiles score 10% more |
| Fog | Rival territory is hidden on the map |
| Landslide | One in twenty of every team's tiles turns ghost on the 1st |

## The leaderboard

Teams are ranked every month on Hold gained, takeovers, ghost tiles reclaimed, new tiles discovered, council seats and bounties. There's also a per-active-member ranking so small teams have something to aim for. Your finishing position earns your team shop points.

---

# FAQ

## Getting started

**How do I join?**
The beta is invite-only. Get a beta code from someone already playing (every player gets three to share), then sign up with a handle and password.

**Do I need to be in a team?**
Yes, to score. Hold belongs to teams. Start your own or join one with its invite code, which the captain can share from the Team page.

**What equipment do I need?**
An Android phone with the free WiGLE WiFi Wardriving app is enough to start. ESP32-based scanners that save WiGLE-format logs (Marauder builds and similar) work too, and are better at picking up 5 GHz.

**Does it work on iPhone?**
iPhones can't scan Wi-Fi like this, so iOS can't record scans. You can still play from an iPhone: view the map, vote and manage your team using files recorded on another device.

## Scanning and uploading

**How do I upload?**
Export your session from WiGLE (or copy the CSV off your scanner), open Upload scans and choose the file. It's checked on your device first, then credited by the server, usually within a few seconds.

**What's the API key for?**
Scanners that can upload by themselves use your personal API key, found under Profile. One key covers all your devices. Treat it like a password: anyone holding it can upload as you. You can make a new one at any time, which stops the old one working.

**Why didn't my upload count?**
The note on the upload says why. The usual reasons:
- The scan is over 72 hours old.
- You'd already counted those networks today.
- You hit the daily Hold limits.
- The GPS track jumped around impossibly. Turn on high-accuracy location and wait for a GPS fix before you start.

**What are the daily limits?**
40 Hold per tile per team, and 10,000 Hold per player per day. Both reset at midnight UTC. The Upload page shows how much you've used.

**Can I upload old drives?**
Only the last 72 hours count. Upload soon after you get home.

**Does it matter how fast I go?**
Walking, cycling and driving all work. Faster means more ground but fewer networks per tile. Trains can trip the GPS checks if the track jumps.

## Playing

**Why is my territory disappearing?**
That's the rot. Everything fades unless it's scanned again. Check Dashboard for tiles about to turn ghost, and keep your territory connected; cut-off pockets rot faster.

**How do I take a tile from another team?**
Scan it. Your gain drains their Hold, and when yours is higher it's yours. Raiders and Anarchists drain hardest.

**What's a ghost tile?**
A tile whose Hold has run out. Nobody owns it, it speeds up rot next to it, and reclaiming it gives bonus Hold.

**How do I get a council seat?**
Own enough of the town: at least 5% of its stake and a place in its top seats. Seats are recalculated as Hold changes, so they can be lost.

**Why can't my team vote?**
Either you don't have a seat in that town, your team is barred after an audit or a no-confidence vote, or your team is Anarchists (who never sit on councils).

**What happens if my town falls?**
The council's laws go, rot runs faster and the biggest stakeholder becomes Warlord. It comes back through reform or restoration, or turns into a Free City after 30 days.

**How do items know I'm really there?**
Firing an item asks for a fresh scan, under 15 minutes old, from where you're standing. It has to hear networks the game already knows in that spot, and each scan can only be used once.

**I'm going away. Will I lose everything?**
Set a personal freeze (Profile) or ask your team for a team freeze (Team). Both start 12 hours after you set them.

## Account and security

**I forgot my password. Can you email me?**
BITROT doesn't store email addresses. You get back in with a passkey, an authenticator app or one of your recovery codes. If you lose all of those, contact the operator, who can issue new recovery codes after checking it's really you.

**Where are my recovery codes?**
They were shown once when you signed up. If you didn't save them, make new ones under Profile → Security. That cancels the old set.

**Should I add a passkey?**
Yes. A passkey (your phone, a fingerprint, or a security key like a YubiKey) can't be phished, and lets you sign in without a password.

**Someone else is logged into my account.**
Profile → Security lists every signed-in session. Sign them all out, change your password and make new recovery codes.

## Privacy

**What do you store about my scans?**
The uploaded file is deleted as soon as it's processed. Network names are never stored, and network addresses are only kept as one-way keyed hashes. Your drive route and individual sightings are deleted after 30 days. What stays is per tile, not per person. The privacy policy has the full details.

**Can other players see where I've been?**
No. They see your handle, your team, the team's tiles and council actions, never your routes or the networks you heard.

**Can I download or delete my data?**
Yes, both from Profile → Security.

## Fair play and safety

**What counts as cheating?**
Faking or editing scans, spoofing GPS, sharing accounts to dodge limits, or uploading someone else's drives. Uploads are checked automatically, suspicious accounts are reviewed, and Hold gained by cheating gets removed.

**Is wardriving legal?**
Passively listening to what networks broadcast publicly is generally lawful in the UK. BITROT never asks you to connect to, access or interfere with any network. Check the law where you play if you're elsewhere.

**Any rules for playing safely?**
- Never use your phone while driving. Let it record on its own, or play as a passenger.
- Don't trespass or go anywhere you wouldn't otherwise be allowed.
- Don't loiter outside people's homes to grab a tile.
- No territory is worth a risk.

## The beta

**Will progress be wiped?**
There's no wipe planned, but it's a beta. Rules and numbers will be tuned, and things may change.

**Why are some things missing?**
Zigbee, LoRa and the materials they give (Wax and Echo), plus the items that need them, arrive later.

**How do I report a bug or give feedback?**
Use the feedback link at the bottom of the menu. Include what you did, what you expected, and the request ID if an error showed one.
****
