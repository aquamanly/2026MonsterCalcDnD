# 5E 2026 Encounter Builder

A comprehensive web-based tool for creating and balancing D&D 5E combat encounters using official 5E 2025 rules combined with 4th Edition tactical design principles.

## Features

### 🎲 Automatic Encounter Generation
Generate balanced encounters automatically based on party level, size, and desired difficulty. Choose from 7 different encounter types inspired by 4e tactical design.

### ⚔️ Custom Monster Creation
Create custom monsters with full stat blocks including AC, HP, Attack Bonus, Damage, and Save DC. Auto-fill stats based on Challenge Rating with optional role modifiers.

### 📊 XP Budget Tracking
Real-time XP budget calculation and tracking using official 5E 2025 encounter balancing rules. Visual indicators show if you're over or under budget.

### 🎭 Monster Roles (4e Style)
Apply tactical roles to monsters that automatically adjust their stats:
- **Brute** - High HP and damage dealers
- **Soldier** - High AC defenders
- **Controller** - Area effects and crowd control
- **Lurker** - Stealth and ambush specialists
- **Artillery** - Ranged damage dealers
- **Minion** - Swarm units with 1 HP
- **Leader** - Buffs and commands allies

### 🌋 Environmental Hazards
Add dynamic environmental challenges to encounters:
- **Light** - Difficult terrain, low obstacles, dim light
- **Moderate** - Pit traps, fire zones, unstable ground, magical darkness
- **Heavy** - Lava pools, collapsing ceilings, poison gas, lightning pillars, freezing winds

## How to Use

### Quick Start: Generate an Encounter

1. **Open the tool** in your web browser
2. **Navigate to the "Generate" tab** (default view)
3. **Set your parameters:**
   - Party Level (1-20)
   - Number of Characters (1-8)
   - Difficulty (Easy, Medium, Hard, Deadly)
   - Encounter Type (see below)
   - Environmental Hazards (None, Light, Moderate, Heavy)
4. **Click "Generate Encounter"**
5. **View your encounter** in the "Current Encounter" section

### Encounter Types Explained

#### Solo/Boss Battle
- One powerful boss creature at 80% of XP budget
- 2-4 minions to support
- **Best for:** Epic showdowns, story climaxes
- **Tactics:** Focus fire on boss, manage minions

#### Horde/Swarm
- 8-12 weak minion creatures
- All have 1 HP (killed by any damage)
- **Best for:** Overwhelming odds, area effect showcases
- **Tactics:** AoE attacks, positioning

#### Wolf Pack/Skirmishers
- 4-6 fast lurker-type enemies
- Hit-and-run tactics, high mobility
- **Best for:** Dynamic combat, chase sequences
- **Tactics:** Preventing escapes, locking down enemies

#### Ambush
- 3 lurkers (hidden attackers)
- 2 controllers (crowd control)
- **Best for:** Surprise attacks, tense encounters
- **Tactics:** Stealth detection, area denial

#### Elite Team/Targeted Strike
- 3-4 specialized enemies
- Each has a different role (soldier, artillery, controller, leader)
- **Best for:** Tactical combat, smart enemies
- **Tactics:** Target priority, disrupting synergies

#### Standard (Balanced Mix)
- 1 leader
- 2 soldiers
- 1 artillery
- 2-4 minions
- **Best for:** Traditional D&D combat, versatile encounters
- **Tactics:** Classic battlefield tactics

#### Stomping Ground (Hazard Focus)
- 3-5 environmental hazards
- 2-4 guardian creatures
- **Best for:** Environmental storytelling, movement-focused combat
- **Tactics:** Terrain manipulation, forced movement

### Manual Monster Creation

1. **Go to the "Create" tab**
2. **Fill in monster details:**
   - Name
   - Challenge Rating (CR)
   - Monster Role (optional, applies stat modifiers)
3. **Click "Auto-Fill from CR"** for baseline stats
4. **Adjust stats manually** if needed
5. **Add details** (special abilities, traits)
6. **Click "Add Monster"**

Your monster is saved to the library and can be added to any encounter.

### Building Custom Encounters

1. **Go to the "Encounter" tab**
2. **Set party parameters:**
   - Party Level
   - Party Size
   - Desired Difficulty
3. **Click "Calculate XP Budget"**
4. **Add monsters from your library** to the encounter
5. **Watch the XP tracker** to stay within budget

## Understanding the Rules

### XP Budget System (5E 2025)

The tool calculates XP budgets based on official 5E 2025 guidelines:

**Easy Encounters:** Characters should win with minimal resource expenditure
**Medium Encounters:** Characters will need to use healing and tactical thinking
**Hard Encounters:** High risk, potential character knockouts
**Deadly Encounters:** Lethal threat, TPK possible without excellent tactics

### Challenge Rating to XP

| CR | XP | CR | XP | CR | XP |
|----|-----|----|----|----|----|
| 0 | 10 | 5 | 1,800 | 10 | 5,900 |
| 1/8 | 25 | 6 | 2,300 | 11 | 7,200 |
| 1/4 | 50 | 7 | 2,900 | 12 | 8,400 |
| 1/2 | 100 | 8 | 3,900 | 13 | 10,000 |
| 1 | 200 | 9 | 5,000 | 14 | 11,500 |
| 2 | 450 | | | 15 | 13,000 |
| 3 | 700 | | | 16+ | See table |
| 4 | 1,100 | | | | |

### Monster Stat Guidelines by CR

The tool follows official 5E 2025 monster creation guidelines:

**CR 0-1:** Basic stats with minimal variation
**CR 2-7:** Stats scale as `Base + (CR ÷ 2)`
**CR 8+:** Linear scaling continues

**Example for CR 5:**
- AC: 13 + (5 ÷ 2) = 15-16
- HP: (15 × 5) + 15 = 90
- Attack: 4 + (5 ÷ 2) = +6 or +7
- Damage: (5 × 5) + 5 = 30 per round
- Save DC: 11 + (5 ÷ 2) = 13-14

### Role Modifiers

Roles adjust the baseline stats to create specialized monsters:

| Role | AC | HP | Attack | Damage | DC |
|------|----|----|--------|--------|-----|
| **Brute** | -2 | ×1.5 | +0 | ×1.5 | +0 |
| **Soldier** | +2 | ×1.2 | +1 | ×0.8 | +0 |
| **Controller** | +0 | ×0.8 | +0 | ×0.8 | +2 |
| **Lurker** | +1 | ×0.8 | +2 | ×1.3 | +1 |
| **Artillery** | -1 | ×0.7 | +1 | ×1.4 | +0 |
| **Minion** | +0 | ×0.05 | +0 | ×0.5 | +0 |
| **Leader** | +1 | ×1.1 | +0 | ×0.9 | +1 |

## Tips for Great Encounters

### Balancing Difficulty

- **Don't rely solely on XP budget** - terrain, tactics, and objectives matter
- **Account for party composition** - ranged-heavy parties struggle with flyers
- **Consider resources** - is this their first fight or fifth today?
- **Test deadly encounters carefully** - they can TPK quickly

### Using Environmental Hazards

- **Hazards reduce creature XP** - the tool accounts for this automatically
  - Light hazards: No reduction
  - Moderate hazards: 20% XP reduction for creatures
  - Heavy hazards: 40% XP reduction for creatures
- **Describe hazards vividly** - make terrain feel real and dangerous
- **Reward creativity** - let players use hazards against enemies
- **Force movement** - hazards make positioning crucial

### Monster Quantity Guidelines

- **Too many monsters?** If you have more than 2× party size, consider using minions
- **Action economy matters** - 8 enemies get 8 attacks vs. party's 4
- **Tracking difficulty** - more than 3 unique stat blocks gets complex
- **CR 0 creatures** - use sparingly, they can bog down combat

### Tactical Tips by Encounter Type

**Solo/Boss:**
- Give the boss legendary actions or lair actions
- Minions prevent focus-fire
- Multiple phases keep it interesting

**Horde:**
- Describe them as a unified mass
- Use group initiative
- Consider morale checks

**Wolf Pack:**
- Emphasize mobility and cunning
- Hit weak targets, avoid tanks
- Retreat and regroup when hurt

**Ambush:**
- Establish surprise rules clearly
- Reward player perception
- Controllers lock down escapes

**Elite Team:**
- Enemies focus fire and combo
- Target squishy characters
- Leader dies last

**Standard:**
- Classic D&D tactics
- Frontline/backline positioning
- Minions protect important targets

**Stomping Ground:**
- Hazards are the real enemy
- Enemies use terrain advantages
- Forced movement is key

## Reference: Monster Manual Integration

This tool is designed to work alongside your Monster Manual. You can:

1. **Import SRD monsters** - manually create entries for commonly used monsters
2. **Modify existing monsters** - adjust stats and add roles to published monsters
3. **Create variants** - make "Goblin Chieftain (Leader)" versions of basic monsters

## Technical Details

### File Structure
- Single HTML file with embedded CSS and JavaScript
- No external dependencies or internet connection required
- All data stored in browser memory (resets on page refresh)

### Browser Compatibility
- Works in all modern browsers (Chrome, Firefox, Safari, Edge)
- Responsive design works on desktop and tablet
- Mobile usable but better on larger screens

### Data Persistence
**Note:** Currently, monsters and encounters are NOT saved between sessions. Refreshing the page will clear all data.

**Workaround:** Keep the tab open during your session, or copy important data to notes.

## Future Feature Ideas

- Export encounters to PDF or JSON
- Import monsters from JSON
- Save encounters to browser localStorage
- Initiative tracker integration
- Monster templates library (dragons, undead, etc.)
- Lair actions and legendary actions builder
- Random name generator
- Encounter difficulty calculator with party composition

## Credits

Created for Dungeon Masters running D&D 5th Edition games.

**Design Philosophy:**
- 5E 2025 official encounter balancing rules
- 4th Edition tactical design principles
- Modern web design for ease of use

## License

Free to use for personal tabletop gaming. Share and modify as you like.

---

## Quick Reference Card

### Default Party: 4 Characters, Level 5, Medium Difficulty
**XP Budget:** 3,000 XP

**Quick Encounters:**
- **Easy Boss Fight:** 1 CR 5 creature (1,800 XP)
- **Medium Challenge:** 2 CR 4 creatures (2,200 XP)
- **Hard Battle:** 1 CR 6 + 2 CR 3 (3,700 XP)
- **Horde:** 12 CR 1/4 minions (600 XP) + 2 CR 3 leaders (1,400 XP)

### Stat Quick Reference (CR 5)
- AC: 15-16
- HP: 80-100
- Attack: +6 to +7
- Damage: 25-35
- Save DC: 13-14

---

**Happy adventuring! May your encounters be balanced and your dice roll high! 🎲**
