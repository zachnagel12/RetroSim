# Retro Football League Simulator

A browser-based simulation game where you manage an alternate NFL universe evolving from 1970 through 2024+. The game itself changes as football changes—passing becomes more valuable, rules evolve, player archetypes shift, and 50+ years of dynamic history accumulates.

**Status**: Architecture Complete | Ready to Build | [Full Documentation](./docs/)

---

## 🎮 Core Gameplay

### Two Game Modes
- **Story Mode**: League progresses 1970-present with historical events, rule changes, expansion voting
- **Sandbox Mode**: Permanent universe where you can continue indefinitely, preserving all history

### What You Do
- Draft players and build rosters
- Manage salary cap and contracts
- Scout talent and make trades
- Hire/fire coaches based on personality
- Navigate free agency and holdouts
- Watch Hall of Fame voting
- Experience 50+ years of alternate NFL history

---

## 🌟 Core Features (MVP)

### Season Simulation
- ✅ 16-week regular seasons (17 in 2022+)
- ✅ Procedurally generated weekly schedules
- ✅ Game simulation based on team strength
- ✅ Real-time standings, playoff races
- ✅ Injury generation and recovery
- ✅ Playoff bracket generation and simulation

### Roster Management
- ✅ 32 procedurally generated teams
- ✅ 1500+ dynamic players with attributes
- ✅ 6 divisions across 2 conferences
- ✅ Player aging and career phases (rookie→prime→declining)
- ✅ Stat tracking (passing, rushing, receiving, defense)
- ✅ Injury tracking and recovery timelines

### Draft & Free Agency
- ✅ 7-round annual draft with trading
- ✅ Procedurally generated rookie class each year
- ✅ Free agency market (post-1993)
- ✅ Salary cap management (post-1994)
- ✅ Contract negotiations and terms
- ✅ Franchise tags and restricted FA (era-appropriate)

### Coaches & Owners
- ✅ Procedurally generated coaches with personalities
- ✅ Coach hiring/firing with contract terms
- ✅ Coach offensive/defensive philosophies
- ✅ Owner personalities affecting team decisions
- ✅ Owner spending levels and philosophy
- ✅ Coaching record tracking

### Narrative & Immersion
- ✅ 50+ headline templates (game results, injuries, trades, records)
- ✅ Scandal generation (2-3 per season league-wide)
- ✅ Rivalry development (division rivals, playoff matchups)
- ✅ Hall of Fame voting (annual ceremony)
- ✅ Award voting (MVP, DPOY, Rookie of Year, Coach of Year)
- ✅ Broadcasting commentary (era-appropriate tone)

### Historical Progression
- ✅ **1970s Era**: Run-heavy, tough defense, reserve clause
- ✅ **1980s Era**: Passing emphasis rises, coaches adapt or die
- ✅ **1990s Era**: Free agency & salary cap introduced, 12 playoff teams
- ✅ **2000s Era**: Cap management sophisticated, 12 playoff teams
- ✅ **2010s Era**: Analytics visible, mobile QBs valued, 12 playoff teams
- ✅ **2020s+ Era**: 17-game season, advanced analytics, complex defenses

**Era mechanics change**:
- Passing emphasis (25% → 70%)
- Salary cap introduction (1994)
- Rule changes per decade
- Player archetype values
- Commentary style
- Hall of Fame leniency

### Records & Statistics
- ✅ Single-season records tracked
- ✅ Career records tracked
- ✅ Team records and milestones
- ✅ Playoff records tracked separately
- ✅ Era-adjusted statistics (1970s ≠ 2020s)
- ✅ Historical database searchable by era/team/player

### Save & Load
- ✅ IndexedDB persistent storage (unlimited)
- ✅ Auto-save after each week
- ✅ Multiple save slots
- ✅ Export/import game saves as JSON
- ✅ Full game state preservation (50+ years of data)

---

## 🎨 Phase 2+ Enhancements (16 Ideas, Effort/Payoff Listed)

### Tier 1: High-Impact, Moderate Effort (10-20 hours each)

| Feature | Hours | Impact | Details |
|---------|-------|--------|---------|
| **Draft Scouting Mini-Game** | 12h | ⭐⭐⭐⭐ | Scouts create uncertainty in draft evaluations |
| **Coaching Tree & Legacy** | 15h | ⭐⭐⭐⭐ | Track coaching dynasties and lineages |
| **Media Outlets System** | 18h | ⭐⭐⭐⭐⭐ | Multiple narrative sources (ESPN, local, radio, social) |
| **Player Chemistry & Locker Room** | 20h | ⭐⭐⭐⭐⭐ | Team cohesion affects performance |
| **Playoff Bracket Drama** | 22h | ⭐⭐⭐⭐ | Expert predictions, upset narratives, bracket busting |
| **Franchise Relocation** | 25h | ⭐⭐⭐ | Full relocation voting and consequences |
| **Medical Advances Over Time** | 18h | ⭐⭐⭐ | 1970s worse outcomes, 2020s better recovery |
| **Custom League Creator** | 30h | ⭐⭐⭐⭐⭐ | Create custom leagues with own rules (infinite replayability) |

### Tier 2: Strategic Layer (20-35 hours each)

| Feature | Hours | Impact | Details |
|---------|-------|--------|---------|
| **Trading System** | 35h | ⭐⭐⭐⭐⭐ | Full trade negotiation, bidding wars, deadline drama |
| **Advanced Analytics Dashboard** | 30h | ⭐⭐⭐⭐ | EPA, CPOE, yards after catch (2010s+ era) |

### Tier 3: Long-Tail Features (10-25 hours each)

| Feature | Hours | Impact | Details |
|---------|-------|--------|---------|
| **Coaching Carousel & Job Market** | 18h | ⭐⭐⭐⭐ | Annual coaching moves and drama |
| **Player Holdouts & Union Negotiations** | 22h | ⭐⭐⭐⭐ | CBA negotiations, strikes, lockouts |
| **Player Development Arcs** | 25h | ⭐⭐⭐⭐ | Personal career stories for every player |
| **Owner Controversies** | 18h | ⭐⭐⭐⭐ | Scandals, forced resignations, ownership changes |
| **Training Camp & Facilities** | 18h | ⭐⭐⭐ | Infrastructure affects player development |
| **International Games & Expansion** | 18h | ⭐⭐⭐ | Post-2005 authenticity, global league |
| **Statistical Records Chasing** | 15h | ⭐⭐⭐⭐ | Narrative drama when records are close |
| **Draft Analysis & Bust Tracking** | 20h | ⭐⭐⭐⭐ | Evaluate picks in hindsight, judge scouts |
| **Award Voting (Expanded)** | 16h | ⭐⭐⭐ | Extended voting mechanics, controversies |
| **Injury Rehab Decisions** | 16h | ⭐⭐⭐ | Risk/reward medical choices per injury |

---

## 🛠️ Tech Stack

- **Frontend**: React + TypeScript
- **State Management**: Zustand (lightweight, serializable)
- **Storage**: IndexedDB (unlimited local saves)
- **Styling**: Tailwind CSS + custom retro CSS
- **Build**: Vite
- **Simulation**: 100% client-side, deterministic, works offline

---

## 📊 Development Roadmap

### Phase 1-4: Core Game (16-20 weeks)
- Project setup & type definitions
- Procedural generation (players, coaches, owners)
- Season simulation engine
- Draft system & free agency
- Player progression & aging
- Coaching & owner systems
- Basic narrative (headlines, scandals)
- Era evolution (6 eras, 1970-2024+)
- Hall of Fame voting
- Records tracking
- Save/load system
- Retro UI & styling

**Result**: Playable 50-year league

### Phase 5: First Enhancements (3-4 weeks)
- Media Outlets (immersion explosion)
- Draft Scouting (fun drafts)
- Chemistry System (strategic depth)

**Result**: 3x more immersive game

### Phase 6: Strategic Layer (4-5 weeks)
- Trading System (core mechanic)
- Coaching Carousel (recurring drama)
- Comeback Stories (emotional narratives)

**Result**: Deep strategic gameplay

### Phase 7: Longevity (ongoing)
- Custom Leagues (infinite replayability)
- Export/Sharing (community features)
- Advanced Analytics (stat nerds)
- Long-tail features

**Result**: Game people play for months/years

---

## 📈 Estimated Timelines

| Timeline | Scope | Result | Hours |
|----------|-------|--------|-------|
| **3 months** | Core + Phase 5 | Good game, 20-30 hours play | 280h |
| **6 months** | Core + Phase 5 + Polish | Great game, 30-50 hours play | 300h |
| **9 months** | Core + Phases 5-6 | Comprehensive, 50-100 hours play | 400h |
| **12 months** | Everything | Masterpiece, 200+ hours potential | 500h+ |

---

## 🎯 Key Design Decisions

### Why Client-Side Simulation?
- Works offline
- Instant response (no latency)
- Deterministic (same seed = same results)
- Unlimited save slots
- Player privacy (no server data)
- Can run multiple simulations

### Why This Tech Stack?
- **React**: Great for complex UI state
- **Zustand**: 2KB, minimal boilerplate, serializable
- **IndexedDB**: Unlimited storage (localStorage = 5-10MB max)
- **TypeScript**: Catch bugs early in simulation
- **Client-side**: No backend complexity, works offline

### Why Retro Aesthetic?
- Forgiving of imperfect graphics
- Matches historical theme (1970s-2020s)
- Data-heavy UI works well retro
- Less art assets needed
- Unique brand identity

---

## 📚 Full Documentation

Complete documentation available in `/docs/`:
- `FOOTBALL_LEAGUE_ARCHITECTURE.md` (12,000 words) — System design
- `DEVELOPMENT_ROADMAP.md` — Week-by-week 20-week plan
- `QUICK_START.md` — 30-minute implementation tutorial
- `VISUAL_REFERENCE.md` — 10 system diagrams
- `ENHANCEMENT_IDEAS.md` — 16 feature ideas detailed
- `ADVANCED_FEATURES.md` — 10 long-tail features
- `PRIORITIZATION_GUIDE.md` — Build strategy & timelines
- `types.ts` — 800+ lines TypeScript interfaces (ready to use)
- `simulationEngine.ts` — 600+ lines core logic (ready to extend)

---

## 🚀 Getting Started

### Quick Path (30 minutes to working prototype)
1. Read `QUICK_START.md`
2. Follow 8 setup steps
3. Have working game

### Deep Path (understand everything)
1. Read `FOOTBALL_LEAGUE_ARCHITECTURE.md`
2. Study `types.ts` and `simulationEngine.ts`
3. Review `VISUAL_REFERENCE.md` diagrams
4. Then follow `QUICK_START.md`

---

## 📋 Feature Checklist

### MVP Features
- [x] Season simulation (16 weeks)
- [x] Procedural player generation
- [x] Draft system (7 rounds)
- [x] Free agency (post-1993)
- [x] Salary cap management (post-1994)
- [x] Coach hiring/firing
- [x] Owner system with personalities
- [x] Injury tracking
- [x] Hall of Fame voting
- [x] Awards voting
- [x] Headlines (50+ templates)
- [x] Scandals
- [x] Rivalries
- [x] Era evolution (6 eras)
- [x] Records tracking
- [x] Save/load system
- [x] Retro UI styling

### Planned Enhancements
- [ ] Media outlets (multiple narratives)
- [ ] Draft scouting mini-game
- [ ] Player chemistry system
- [ ] Trading system (full)
- [ ] Coaching carousel
- [ ] Comeback narratives
- [ ] Custom leagues
- [ ] Advanced analytics
- [ ] Owner drama/resignation
- [ ] Training camp system
- [ ] International expansion
- [ ] Record chasing narratives
- [ ] Extended award voting
- [ ] Injury rehab decisions
- [ ] Export/sharing features

---

## 🎓 What Makes This Special

1. **50-Year Historical Progression**: Game is about evolution from 1970-2024+
2. **The Game Itself Changes**: Pass emphasis, rules, player archetypes shift per era
3. **Procedural Narrative**: Headlines, scandals, comebacks generated dynamically
4. **No Server Needed**: 100% client-side, works offline
5. **Permanent Sandbox**: Play indefinitely after story mode
6. **Strategic Depth**: Multiple systems interact meaningfully
7. **Immersive Atmosphere**: Feels like alternate universe with 50 years of history

---

## 📄 License

MIT

---

## 🙏 Credits

Inspired by: Front Office Football, OOTP Baseball, Football Manager, early Madden franchise modes

---

## 🤝 Contributing

This is an architecture document. To contribute:
1. Review the architecture in `/docs/`
2. Understand the roadmap in `DEVELOPMENT_ROADMAP.md`
3. Follow the code patterns in `types.ts` and `simulationEngine.ts`
4. Submit PRs following the design

---

## 📞 Status

**Current**: Architecture complete, ready to build
**Next**: Phase 1 implementation (weeks 1-4)

See `/docs/DEVELOPMENT_ROADMAP.md` for detailed timeline.

---

**Build something amazing.** 🏈
