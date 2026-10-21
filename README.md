# Tour Sim — golf simulator (fan-made)

A browser golf simulator with **no characters**, just the ball, tee, mat, course, tracer and a launch monitor. **[Play it](https://jamesgregory5-svg.github.io/tour-sim/)**.

The whole game is one self-contained `index.html`, about 1.7 MB, that makes **no network requests**. You can also download it and open it straight from disk (`file://`), which is handy where github.io is blocked. It works on phone and desktop with touch, mouse or keyboard.

> Fan-made; layouts approximate; not affiliated with any club.

## Modes
- **Play a course.** Choose from the top 25 of Golf Digest's *America's 100 Greatest Courses (2025-26)*, plus **Lookaway Golf Club** (Buckingham, PA), which is pinned as the home course. You can play the Front 9, the Back 9 or all 18, from any of the course's real tee sets (tee markers move, and records are kept per course and per tee). Rounds save automatically and can be resumed.
- **Pass-and-play.** 1-4 named players share one device in stroke play. Honors decide who tees off, the player farthest from the hole plays next, and a "Player up" banner shows whose turn it is. Each player has their own ball and name tag. The scorecard and leaderboard cover every player, and a results screen appears at the end. Records are saved under each player's name.
- **Replays.** After a great shot (a hole-out, an eagle or better, inside 6 ft from 100+ yds, a made putt over 30 ft, or a top-5 drive) you're offered a cinematic replay with slow motion near the hole. Tap to skip. **Replay last shot** is always available.
- **Driving range.** Target flags from 50 to 300 yds. It shows dispersion by club, saved **My Bag** gapping and session stats.
- **Closest to the Pin.** A daily seeded famous par 3 with 5 balls.
- **Long Drive.** A daily seeded grid and wind, with 6 balls and the driver only.
- **My Records.** Best 18 and best 9 for each course, a best-ball card, your average, rounds played, aces, longest drive, CTP, fairway/GIR stats and round history with full scorecards.

## Controls
- **Aim:** drag sideways, use the arrow keys, or A/D.
- **Club:** tap a club chip, or W/S. The recommended club is highlighted, and the label shows its predicted carry and total.
- **Swing (timed meter):** tap, click or press Space to start the backswing. Tap again to set the power, then tap a third time as the needle returns to the white sweet-spot line. An early or late third tap gives a push, pull or mishit.
- **Putting:** the green grid shows flowing slope arrows. Tap to start, then tap to strike. Distance is shown in feet.
- **Shape:** 1-5 or the buttons (straight, draw, fade, high, low). **V** changes the view; **C** opens the card.

## Simulation
- **Ball flight.** Drag plus Magnus lift, a tilted spin axis (face-to-path), gear effect, and wind that varies with height.
- **Bounce and roll** depend on the surface: fairway, rough, deep rough or fescue, sand, fringe, green and water.
- **Real terrain.** Every course uses a USGS 3DEP bare-earth elevation grid of about 8 × 10 yd, smoothed and compressed into the file. The terrain affects:
  - the 3D view
  - where the ball lands (flight meets the actual ground)
  - bounce and roll on slopes
  - **lies** (uphill, downhill, ball above or below your feet change launch and curve)
  - **"plays like"** yardage
  - the green tilt fed into the putting grid
- **Micro-undulation** is added on top of the terrain.
- **Launch monitor.** Ball speed, club speed, smash, launch and spin fill in at impact. Carry, total, side, apex and the shape label fill in when the ball lands.

## Courses and data sources
Hole routing, greens, fairways, bunkers, tees, water and woods come from **OpenStreetMap** (© OpenStreetMap contributors, ODbL). Elevation comes from **USGS 3DEP** (public domain). Per-hole par and yardage come only from published scorecards (sources below); none of them are invented. Pin positions, green contours and individual filler trees are generated, and so is any feature missing from OSM (noted in the game). Pebble Beach's seawall and Oakmont's Church Pews are drawn from the OSM shapes.

| Rank | Course | Location | Par | Yards (tees) | Scorecard source |
|---|---|---|---|---|---|
| Home | Lookaway Golf Club | Buckingham, PA | 72 | 6907 (Black) | GolfPass scorecard (Black/Blue/Silver/Gold); hole notes golfcoursebrowser/OSM |
| 1 | Pine Valley Golf Club | Pine Valley, NJ | 70 | 7197 (Back) | BlueGolf / GolfCore scorecard |
| 2 | Augusta National Golf Club | Augusta, GA | 72 | 7555 (Tournament) | Wikipedia (Augusta National GC scorecard) |
| 3 | Cypress Point Club | Pebble Beach, CA | 72 | 6552 (Championship) | Wikipedia (Cypress Point Club scorecard) |
| 4 | Shinnecock Hills Golf Club | Southampton, NY | 70 | 6940 (Red) | Wikipedia (Shinnecock Hills scorecard) |
| 5 | Oakmont Country Club | Oakmont, PA | 71 | 7431 (Championship) | Wikipedia (Oakmont CC scorecard) |
| 6 | Merion Golf Club (East) | Ardmore, PA | 70 | 6946 (Championship) | Wikipedia (Merion GC scorecard) |
| 7 | National Golf Links of America | Southampton, NY | 72 | 6935 (Red) | BlueGolf scorecard |
| 8 | Sand Hills Golf Club | Mullen, NE | 71 | 7089 (Black) | Wikipedia (Sand Hills GC scorecard) |
| 9 | Pebble Beach Golf Links | Pebble Beach, CA | 71 | 7075 (U.S. Open) | Wikipedia (Pebble Beach GL scorecard, 2019 U.S. Open par 71) |
| 10 | Fishers Island Club | Fishers Island, NY | 70 | 6597 (Black) | BlueGolf / Stymie scorecard |
| 11 | Chicago Golf Club | Wheaton, IL | 70 | 6950 (Championship) | Wikipedia (Chicago GC course table) |
| 12 | Seminole Golf Club | Juno Beach, FL | 72 | 7259 (Gold) | BlueGolf / Stymie scorecard |
| 13 | Winged Foot Golf Club (West) | Mamaroneck, NY | 70 (member tees 72) | 7477 (U.S. Open); Blue 7426, Black 6937, White 6522 | Wikipedia (2020 U.S. Open card); GolfPass / Zomma member scorecard |
| 14 | Friar's Head | Baiting Hollow, NY | 71 | 7071 (Back) | golfcoursebrowser / 18Birdies scorecard |
| 15 | Crystal Downs Country Club | Frankfort, MI | 70 | 6509 (Blue) | GolfPass / Zomma scorecard (Blue) |
| 16 | Los Angeles Country Club (North) | Los Angeles, CA | 70 | 7423 (U.S. Open) | Wikipedia (2023 U.S. Open course layout) |
| 17 | The Country Club (Main) | Brookline, MA | 70 | 7264 (U.S. Open) | Wikipedia (2022 U.S. Open course layout) |
| 18 | Riviera Country Club | Pacific Palisades, CA | 71 | 7322 (Genesis) | Wikipedia (Riviera CC scorecard) |
| 19 | Muirfield Village Golf Club | Dublin, OH | 72 | 6739 (Blue) | Wikipedia (Muirfield Village scorecard) |
| 20 | Oakland Hills Country Club (South) | Bloomfield Hills, MI | 72 | 7509 (Black) | Wikipedia (Oakland Hills South scorecard, member par) |
| 21 | Oak Hill Country Club (East) | Rochester, NY | 70 | 7394 (PGA) | Wikipedia (2023 PGA Championship course layout) |
| 22 | Peachtree Golf Club | Atlanta, GA | 72 | 7408 (Championship) | BlueGolf / GolfCore scorecard |
| 23 | Pacific Dunes | Bandon, OR | 71 | 6633 (Black) | Wikipedia (Bandon Dunes Resort scorecards) |
| 24 | Shadow Creek | North Las Vegas, NV | 72 | 7560 (Championship) | BlueGolf / GolfLink scorecard |
| 25 | Prairie Dunes Country Club | Hutchinson, KS | 70 | 7068 (Gold) | GolfPass scorecard (Gold) |

## Known approximations
- **The Country Club:** the US Open composite routing (holes 10-12) is stitched from OSM Main-course holes.
- **OSM par differences:** a few OSM hole lines carry a different par than the scorecard. The scorecard is always used.
- **Synthesized features:** where OSM lacks a green or fairway (for example Prairie Dunes 6), a plausible one is synthesized and flagged.
- **Tee sets:** only tee sets with a published scorecard are offered; several courses currently have one tee set.
- **Tee placement:** tees are placed on land so the tee-to-pin distance matches the scorecard yardage.
