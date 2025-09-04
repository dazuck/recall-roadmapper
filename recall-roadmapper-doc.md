# Recall Roadmapper
## Strategic Visual Roadmapping Tool

### MVP-First Development Strategy

**Core Principle:** Ship the orbital roadmapping experience in 3 weeks, validate with users, then progressively enhance based on actual usage and demand.

**What We're Building First (MVP):**
- ✅ Visual canvas with orbital confidence metaphor
- ✅ Goal and solution management
- ✅ Local storage (no backend needed)
- ✅ Export and share capabilities
- ✅ Single-user experience

**What We're Intentionally Deferring:**
- ❌ User authentication (Phase 6)
- ❌ Real-time collaboration (Phase 6)
- ❌ Team management (Phase 6)
- ❌ Backend infrastructure (Phase 4)
- ❌ Enterprise features (Phase 6+)

**Why This Approach:**
1. **Validate core concept fast** - Is the orbital metaphor intuitive?
2. **Reduce complexity** - No auth = faster development
3. **Lower costs** - $15K vs $92K initial investment
4. **Learn from users** - Build what they actually need
5. **Progressive enhancement** - Add complexity only when validated

### The Problem We're Solving

Every week, teams gather around spreadsheets, Linear boards, and Figma mockups trying to answer the same questions: What are we building? Why are we building it? Who is it for? The tools we use force us into feature lists when we should be discussing goals. They demand false precision with dates when we should be acknowledging uncertainty. They hide the "why" behind the "what."

**Recall Roadmapper** is different. It's a visual canvas where strategy lives as a spatial experience, not a database. Goals anchor the space like gravitational centers, with potential solutions orbiting them at distances that represent our confidence. It's built on a simple insight: the further away something is from a goal, the less certain we are about it. This physical metaphor makes abstract confidence tangible.

---

## Core Philosophy: Goals as Gravity

Imagine your product strategy as a universe. Goals are stars—massive, luminous, pulling everything toward them. Solutions are planets orbiting these stars, held by gravitational pull. The stronger our confidence in a solution, the tighter its orbit. Components and experiments are moons, visible only when you get close enough to see the details.

This isn't just a pretty metaphor. It fundamentally changes how teams think about roadmapping:

1. **Goals become immovable anchors** - You can't accidentally drift into feature factory mode when every solution visually orbits a goal.

2. **Uncertainty becomes visible** - A solution floating far from its goal sends a clear signal: "We're not sure about this yet."

3. **Relationships become obvious** - Solutions cluster around their goals naturally, making trade-offs and priorities self-evident.

4. **Zoom reveals intention** - Zooming out shows strategy; zooming in shows tactics. The right information appears at the right altitude.

---

## The Canvas Model

### Not a Grid, But a Landscape

Unlike traditional roadmap tools with rigid rows and columns, Recall Roadmapper provides an open canvas with **suggested regions**. Think of it like a map with countries rather than a spreadsheet with cells.

The canvas is divided into:
- **Four horizontal swim lanes** for stakeholder groups (these create visual organization but don't constrain positioning)
- **Three vertical phase bands** (Now, Next, Later) that suggest timeline without enforcing rigid placement

Goals can be positioned **anywhere** within this landscape. Want to place a goal at the boundary between "Now" and "Next" to show transition? Go ahead. Need to cluster related goals even if they're for different stakeholders? The canvas allows it.

```
The Canvas Landscape:
┌─────────────────────────────────────────────────────────┐
│                          NOW                            │
│  Free-to-Play ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─  │
│     (100%)         ⭐ (placed freely)                   │
│                   ·⚪⚪·                                 │
│  Staked ─ ─ ─ ─ ─ ─ ╱ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─  │
│   (90%)           ⭐        ⭐ (near boundary)           │
│                  ⚪·        ·⚪⚪                         │
│  Curators ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─  │
│    (9%)                                                 │
│                                                         │
│  Developers ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─  │
│    (1%)            ⭐                                   │
│                   ⚪⚪·                                  │
└─────────────────────────────────────────────────────────┘
        NOW      │      NEXT      │      LATER
```

The swim lanes and phases provide **visual anchoring** without rigid constraints. Goals naturally cluster in their stakeholder lanes, but can drift toward boundaries when they serve multiple groups. They tend toward their phase band, but can straddle boundaries when timing is fluid.

---

## Visual Design Language

### Goals: The Strategic Anchors

Goals are the stars of our universe—impossible to miss, pulling everything toward them. Visually, they're substantial cards with depth and presence:

```
╔════════════════════════════════╗
║ 🎯 Increase Curation Activity   ║  ← Clear, action-oriented title
║ ────────────────────────────    ║
║ Drive 10x more quality ratings  ║  ← The "why" in one line
║ to improve model ranking        ║
║                                 ║
║ Progress: ●●●○○ 60%            ║  ← Visual progress
║ Owner: Sarah | Curators         ║  ← Accountability
║ [Decided] Q2 Priority          ║  ← State and context
╚════════════════════════════════╝
```

Each goal uses color from its stakeholder palette, but with enough variation to avoid monotony. Size scales with priority—P1 goals are visually larger, demanding attention. A subtle shadow gives them elevation above the canvas, reinforcing their importance.

### Solutions: Orbital Bets

Solutions orbit their parent goals in concentric rings representing confidence levels:

- **Inner orbit (80-100% confidence)**: "We're committed to this approach"
- **Middle orbit (50-79% confidence)**: "This looks promising, still validating"  
- **Outer orbit (<50% confidence)**: "Early exploration, might not work"

The physics matter here. Solutions don't just float randomly—they maintain stable orbits. You can drag a solution closer or further from its goal, and it snaps to the appropriate confidence ring. Multiple solutions at the same confidence level distribute evenly around the orbit, like electrons in a shell.

```
         ⚪ Gamification
            ╲ 
     ⚪────────⭐────────⚪
  AI Coach   Goal   Better Onboarding
              │
         ⚪ Incentives
```

Solutions themselves are circles sized by effort (S/M/L) with small badges indicating impact (🔥⚡💧). Their color saturation shows state—exploring solutions are outlined, evaluating solutions are partially filled, committed solutions are solid.

### Components: Implementation Details

Components and experiments are the finest level of detail—tiny dots when zoomed out, expanding to readable cards when you focus on their parent solution. They cluster naturally around their solution like moons around a planet, using physics simulation to avoid overlaps while staying visually associated.

---

## The Power of Semantic Zoom

### Three Altitudes of Understanding

The zoom isn't just about making things bigger or smaller—it's about showing different information at different altitudes, like how a map shows countries at one zoom level and streets at another.

#### Altitude 1: Strategic Overview (30,000 feet)
At maximum zoom-out, you see the entire landscape. Goals are visible as titled cards, but solutions appear as simple counts or small dots. The focus is entirely on strategic alignment:
- Which stakeholder groups have goals?
- How are priorities distributed across phases?
- Are we balanced or over-indexed somewhere?

This is the view for board meetings and quarterly planning. A CEO can understand the entire strategy in seconds.

#### Altitude 2: Tactical Planning (10,000 feet)
Zoom in on a region, and solutions become visible with their labels. You can see confidence rings, understand the bets we're making, and how they relate to goals. This is where most product discussions happen:
- What solutions are we considering for each goal?
- How confident are we in each approach?
- Where do we have too many bets? Too few?

Product managers live at this altitude, making trade-offs and adjusting confidence levels.

#### Altitude 3: Implementation Detail (Ground level)
Focus on a specific solution, and components bloom into view. Now you see the actual work—experiments to run, features to build, integrations needed. Linear links become visible. Owner assignments appear. This is where planning becomes execution.

Engineers zoom here to understand what needs building. Designers zoom here to see what needs designing.

### The Zoom Experience

Zooming isn't jarring—it's smooth and intentional. As you zoom toward a goal, other goals fade to 30% opacity, keeping context while reducing distraction. The selected goal grows, its solutions spread out for clarity, and previously hidden details fade in.

Double-clicking a goal triggers an animated zoom that takes exactly 800ms—long enough to maintain spatial context, fast enough to feel responsive. The physics engine ensures solutions maintain their relative positions during zoom, preventing disorientation.

---

## Interaction Design

### Direct Manipulation

Everything on the canvas responds to direct manipulation. This isn't a form-based editor where you click "Edit" and fill in fields. You grab things and move them:

- **Drag a goal** to a new position on the canvas
- **Drag a solution** radially to adjust confidence (closer = more confident)
- **Drag a solution** tangentially to reorder within its confidence ring
- **Drag components** to reorganize around their solution

The canvas provides immediate visual feedback. As you drag a solution toward its goal, ghost rings appear showing the confidence levels. Release, and the solution animates into its new orbit. It feels physical, like moving pieces on a board.

### Decision Logging: The Two-Click Truth

One of our core principles is preserving the "why" behind decisions. Every state change requires a rationale, captured in just two clicks:

**Click 1**: Click the state badge on any item  
**Click 2**: Select new state and type a one-line rationale

That's it. The system automatically captures:
- Timestamp
- Who made the decision
- Previous state
- New state
- The rationale

These decisions form an immutable audit log. You can't edit history—you can only add new decisions. This creates a trail of thought that survives personnel changes and forgotten context.

```
Decision Log for "Gamification Solution":
┌──────────────────────────────────────────────────┐
│ Mar 15, 2:30pm - Sarah Chen                     │
│ Exploring → Evaluating                          │
│ "User research shows strong engagement signal"   │
├──────────────────────────────────────────────────┤
│ Mar 22, 4:15pm - Marcus Smith                   │
│ Evaluating → Committed                          │
│ "Prototype testing hit 85% satisfaction target" │
└──────────────────────────────────────────────────┘
```

### Keyboard-First Power Users

While the visual interface is primary, power users can navigate entirely via keyboard:

**Navigation**
- `Space` + drag: Pan around canvas
- `Z` / `X`: Zoom in/out
- `Tab`: Cycle through goals
- `1-4`: Jump to stakeholder lane
- `/`: Quick search with spatial results

**Creation**
- `N`: New goal at cursor
- `B`: New bet (solution) for selected goal
- `C`: New component for selected solution
- `D`: Open decision log

**View Control**
- `F`: Toggle filters panel
- `H`: Show/hide dependencies
- `M`: Enter meeting mode
- `E`: Export current view

The shortcuts follow familiar patterns from design tools (space for pan) and code editors (/ for search), reducing the learning curve.

---

## Core Features in Context

### The Linear Handoff

Recall Roadmapper is explicitly **not** a project management tool. It's where strategy is formed, not where tasks are tracked. Linear remains the source of truth for execution. But the handoff between strategy and execution must be seamless.

When zoomed into implementation details, each component can be linked to a Linear issue with a single click. The link is one-way—we store Linear's ID and deep-link out to it, but we don't try to sync state bidirectionally. Why? Because strategy and execution move at different speeds. A solution might be "Committed" strategically while its Linear tasks are still in backlog.

The handoff includes context: the goal's "why," the solution's confidence level, and the complete decision history. An engineer opening a Linear ticket can click back to understand the full strategic context in seconds.

### Meeting Mode: From Discussion to Decision

Traditional roadmap reviews involve someone sharing their screen, walking through items, and hopefully remembering to update the document afterward. Meeting Mode changes this dynamic.

When you start Meeting Mode, the canvas takes a snapshot. As the meeting progresses, participants can propose changes directly on the canvas—these appear as "diffs" with a subtle animation. Each diff is queued in a panel:

```
Proposed Changes:
┌────────────────────────────────────────┐
│ 1. Move "AI Coach" to inner orbit     │
│    Proposed by: Marcus                │
│    Rationale: "ML prototype working"  │
│    [Accept] [Decline] [Discuss]       │
├────────────────────────────────────────┤
│ 2. Add "Tutorial System" solution     │
│    Proposed by: Janet                 │
│    Rationale: "Addresses drop-off"    │
│    [Accept] [Decline] [Discuss]       │
└────────────────────────────────────────┘
```

The meeting owner can accept or decline each change. Accepted changes apply immediately with automatic decision logging. At meeting end, export a summary of all decisions made. No more "What did we decide?" follow-ups.

### Filters and Views

Not everyone needs to see everything. A developer might only care about technical goals in the "Now" phase. A marketer might focus on go-to-market solutions that are "Decided." Views make this possible:

- Filter by stakeholder, phase, state, owner, or tags
- Save view configurations with shareable URLs
- Export views as PNG/PDF with presets:
  - "Executive Summary" (goals only, all phases)
  - "Sprint Planning" (Next phase, all details)
  - "Team Deep-Dive" (single stakeholder, all details)

Views aren't just about hiding items—they adjust the canvas layout to use space efficiently, ensuring the filtered content remains scannable and well-organized.

---

## Development Environment Setup

### MVP Prerequisites (Minimal)
```bash
# Required software versions
Node.js 20.0+ 
npm 9.0+
Git 2.40+
# That's it! No database or Redis needed for MVP
```

### MVP Local Development (Phase 1-3)

**1. Clone and Install:**
```bash
# Clone repository
git clone https://github.com/recall/roadmapper.git
cd roadmapper

# Install dependencies
npm install

# No environment variables needed for MVP!
```

**2. Start Development:**
```bash
# Single command to start
npm run dev

# Opens at http://localhost:5173
# Hot reload enabled
# No backend needed
```

**3. Build for Production:**
```bash
# Build static site
npm run build

# Preview production build
npm run preview

# Deploy to Vercel/Netlify
npm run deploy
```

### Future Backend Setup (Phase 4+)

**Only when needed:**
```bash
# Phase 4: Add simple backend
npm install express cors jsonwebtoken bcrypt
npm install --save-dev @types/express

# Phase 5: Add database
docker run -p 5432:5432 postgres:15
npm install prisma @prisma/client

# Phase 6: Add real-time
npm install socket.io redis
```

### Development Workflow

**Git Branching Strategy:**
- `main` - Production-ready code
- `develop` - Integration branch
- `feature/*` - New features
- `fix/*` - Bug fixes
- `release/*` - Release preparation

**Commit Convention:**
```bash
feat: Add orbital physics simulation
fix: Resolve zoom performance issue
docs: Update API documentation
test: Add goal creation tests
refactor: Simplify canvas rendering
```

### Code Quality Tools

```json
// package.json scripts
{
  "lint": "eslint . --ext .ts,.tsx",
  "format": "prettier --write .",
  "type-check": "tsc --noEmit",
  "test": "vitest run",
  "test:watch": "vitest watch",
  "test:e2e": "playwright test",
  "pre-commit": "lint-staged"
}
```

## Testing Strategy

### Testing Pyramid

**1. Unit Tests (60% coverage target)**
```typescript
// Example: Testing orbital physics
describe('OrbitalPhysics', () => {
  it('should calculate correct orbit radius based on confidence', () => {
    const confidence = 75;
    const radius = calculateOrbitRadius(confidence);
    expect(radius).toBe(MIDDLE_ORBIT_RADIUS);
  });
});
```

**2. Integration Tests (30% coverage)**
- API endpoint testing with Supertest
- Database operations with test transactions
- WebSocket event testing
- Canvas rendering with snapshot tests

**3. E2E Tests (10% coverage)**
```typescript
// Playwright example
test('user can create and position a goal', async ({ page }) => {
  await page.goto('/roadmap/123');
  await page.click('[data-testid="new-goal"]');
  await page.fill('[name="title"]', 'Increase User Engagement');
  await page.dragAndDrop('[data-testid="goal-1"]', '[data-testid="canvas"]');
  expect(await page.locator('[data-testid="goal-1"]')).toBeVisible();
});
```

### Performance Testing

```javascript
// Load testing with k6
export default function() {
  const payload = JSON.stringify({
    goalId: '123',
    position: { x: 100, y: 200 }
  });
  
  const response = http.post('http://localhost:3001/api/goals/move', payload);
  check(response, {
    'status is 200': (r) => r.status === 200,
    'response time < 200ms': (r) => r.timings.duration < 200
  });
}
```

### Quality Gates

**CI Pipeline Requirements:**
- All tests must pass
- Code coverage > 70%
- No critical security vulnerabilities
- Lighthouse score > 85
- Bundle size < 500KB

## Implementation Strategy - MVP First Approach

### Core Principle: Ship Fast, Iterate Based on Usage

We're prioritizing the core visual roadmapping experience and deferring complex features like authentication, real-time collaboration, and advanced integrations until we validate the core concept with users.

### MVP Scope (Weeks 1-3)

**IN SCOPE:**
- Canvas with orbital visualization
- Goal and solution management  
- Drag-and-drop positioning
- Confidence levels via orbital distance
- Basic export (PNG/JSON)
- Local storage persistence
- Single-user experience

**OUT OF SCOPE (Deferred):**
- Authentication/authorization
- Real-time collaboration
- Team management
- Meeting mode
- Linear integration
- Comments and @mentions
- Advanced permissions

### Phase 0: Lightweight Setup (2 days)

**Simplified Technical Setup:**
1. Single repository with simple structure
2. Basic GitHub Pages deployment
3. Local storage for data persistence
4. No backend initially (static site)
5. No authentication needed

**Deliverables:**
- Working local development
- Deployed static site
- Basic project structure

### Phase 1: Core Canvas MVP (Week 1)

Focus entirely on proving the orbital visualization concept works.

**Day 1-2: Canvas Foundation**
- Pixi.js setup with pan/zoom
- Basic rendering pipeline
- Canvas controls (zoom buttons, reset view)

**Day 3-4: Goals & Orbits**
- Goal cards (draggable)
- Orbital physics (three confidence rings)
- Visual feedback on drag

**Day 5: Solutions**
- Solution nodes
- Confidence-based positioning
- Basic state management

**Success Criteria:** 
- Orbital metaphor feels intuitive
- Smooth performance with 50+ nodes
- Basic roadmap creation works

### Phase 2: Core Features (Week 2)

Complete the essential roadmapping features without external dependencies.

**Day 1-2: Semantic Zoom**
- Three zoom levels (overview, planning, detail)
- Progressive detail disclosure
- Smooth transitions

**Day 3: Decision Logging**
- State changes with rationales
- Local storage persistence
- History view panel

**Day 4: Components Layer**
- Sub-items under solutions
- Nested visualization
- Basic clustering

**Day 5: Export & Share**
- Export to PNG
- Export to JSON
- Share via URL (with embedded data)

**Success Criteria:**
- Complete roadmaps can be created and shared
- Zoom reveals appropriate detail at each level
- Data persists between sessions

### Phase 3: Polish & Public Launch (Week 3)

**Day 1-2: UI Polish**
- Keyboard shortcuts
- Context menus
- Improved visual design
- Mobile view (read-only)

**Day 3: Import Data**
- CSV import template
- JSON import
- Sample roadmaps

**Day 4-5: Launch Prep**
- Landing page
- Documentation
- Video tutorial
- Analytics setup

**Deliverables:**
- Public URL (roadmapper.recall.ai)
- Complete documentation
- 3 sample roadmaps
- Usage analytics

---

## Post-MVP Phases (Based on User Feedback)

### Phase 4: Backend & Persistence (Week 4-5)

**Only implement if users request:**
- User accounts (simple email/password)
- Cloud data storage
- Multiple roadmaps per user
- Basic versioning

**Simplified Backend:**
- Node.js + Express
- PostgreSQL (single table initially)
- JWT for sessions
- Heroku/Railway deployment

### Phase 5: Collaboration (Week 6-7)

**Only if validated need:**
- View-only sharing with link
- Comments on goals
- Basic permissions (owner/viewer)
- Change notifications

**Note:** Real-time collaboration deferred until strong demand

### Phase 6: Enterprise Features (Month 2+)

**Advanced features for paying customers:**
- SSO/SAML authentication
- Team workspaces
- Real-time collaboration
- Meeting mode
- Linear/Jira integration
- Advanced permissions
- Audit logs
- API access

---

## Simplified Tech Stack for MVP

### MVP Stack (Weeks 1-3)

**Frontend Only:**
- **Framework:** React with TypeScript
- **Canvas:** Pixi.js
- **State:** Zustand
- **Styling:** Tailwind CSS
- **Build:** Vite
- **Hosting:** Vercel/Netlify (free tier)
- **Storage:** LocalStorage + IndexedDB

**No Backend Required:**
- Data stored locally in browser
- Share via URL with encoded data
- No user accounts
- No team features
- No real-time sync

### Progressive Enhancement Strategy

Start with static site, add backend only when needed:

```javascript
// Phase 1-3: Local storage only
const storage = {
  save: (data) => localStorage.setItem('roadmap', JSON.stringify(data)),
  load: () => JSON.parse(localStorage.getItem('roadmap'))
}

// Phase 4+: Add API when needed
const api = {
  save: async (data) => {
    if (user.isAuthenticated) {
      await fetch('/api/roadmap', { method: 'POST', body: data })
    } else {
      storage.save(data)
    }
  }
}
```

---

## Technical Architecture

### Tech Stack & Infrastructure

**MVP Stack (Phase 1-3) - What We're Actually Building First:**
```javascript
// Entire tech stack for MVP
{
  "frontend": {
    "framework": "React 18 + TypeScript",
    "canvas": "Pixi.js v7",
    "state": "Zustand (local only)",
    "styling": "Tailwind CSS",
    "build": "Vite"
  },
  "backend": null, // No backend for MVP!
  "database": "LocalStorage + IndexedDB",
  "hosting": "Vercel/Netlify (free)",
  "auth": null, // No auth for MVP!
  "cost": "$0-10/month"
}
```

**Future Full Stack (Phase 4-6) - Only If Validated:**
```javascript
// Progressive enhancement based on user demand
{
  "phase4": {
    "backend": "Node.js + Express",
    "database": "PostgreSQL",
    "auth": "Simple JWT"
  },
  "phase5": {
    "sharing": "Read-only links",
    "comments": "Basic threading"
  },
  "phase6": {
    "realtime": "Socket.io + Redis",
    "enterprise": "SSO/SAML",
    "infrastructure": "AWS ECS + CloudFront"
  }
}
```

**Why This Approach:**
- **Ship in 3 weeks** instead of 6-8 weeks
- **$15K budget** instead of $92K
- **Validate core UX** before building infrastructure
- **No technical debt** - start simple, enhance progressively

### Why Canvas, Not DOM

We chose canvas rendering (Pixi.js/Konva) over DOM manipulation for several reasons:

1. **Performance at scale**: 300+ nodes with physics simulation would kill DOM performance
2. **Smooth zooming**: Canvas gives us pixel-perfect control over zoom/pan
3. **Custom rendering**: Orbital layouts and particle effects are natural in canvas
4. **Future-proofing**: Advanced features like dependency routing need canvas flexibility

### Data Model Philosophy

The data model is intentionally simple and flexible. Rather than a complex relational structure, we use a document-based approach with denormalized data:

```typescript
// Core entity - everything else attaches to goals
interface Goal {
  id: UUID
  title: string
  why: string                  // One-line purpose
  stakeholder: StakeholderGroup
  phase: Phase                 // Suggested, not enforced
  position: {x: number, y: number}  // Absolute canvas position
  priority: 1 | 2 | 3
  state: 'exploring' | 'decided' | 'done'
  owner: User
  progress: number
  
  // Denormalized for performance
  solutions: Solution[]
  decisions: Decision[]
  comments: Comment[]
}

// Solutions know their orbit position
interface Solution {
  id: UUID
  title: string
  confidence: number  // 0-100, determines orbit distance
  angle: number      // Position on orbit circumference
  effort: 'S' | 'M' | 'L'
  impact: 'H' | 'M' | 'L'
  state: State
  
  // Denormalized
  components: Component[]
}

// Decisions are immutable
interface Decision {
  id: UUID
  timestamp: Date
  author: User
  fromState: State
  toState: State
  rationale: string
  readonly immutable: true  // TypeScript marker
}
```

This denormalized approach means:
- Single query to load a goal with all its data
- No complex joins for rendering
- Easy to cache and optimize
- Natural fit for real-time updates

### Real-Time Sync Strategy

Real-time collaboration uses operational transformation (OT) for position updates and last-write-wins (LWW) for properties:

- **Positions**: OT ensures smooth dragging without conflicts
- **Properties**: LWW with optimistic UI updates
- **Decisions**: Append-only, no conflicts possible
- **Presence**: Ephemeral WebSocket data, not persisted

### Authentication & Authorization (DEFERRED TO PHASE 6)

**MVP Approach (Phases 1-3):**
- **No authentication required**
- **Local storage only**
- **Share via URL with embedded data**
- **No user accounts**
- **No team features**

**Future Authentication (Phase 6+):**
When validated by enterprise customer demand:

```typescript
// Phase 6: Enterprise authentication
enum Role {
  OWNER = 'owner',      // Full control
  ADMIN = 'admin',      // All editing
  EDITOR = 'editor',    // Create/edit/delete
  VIEWER = 'viewer'     // Read-only
}

// Start simple, expand based on needs
interface MVPAuth {
  email: string
  password: string  // Phase 4
}

interface EnterpriseAuth {
  sso: boolean      // Phase 6
  saml: boolean     // Phase 6
  mfa: boolean      // Phase 6
}
```

**Progressive Authentication Strategy:**
1. **Phase 1-3:** No auth, local storage
2. **Phase 4:** Simple email/password
3. **Phase 5:** Basic sharing permissions
4. **Phase 6:** Enterprise SSO/SAML/MFA

### API Design

**RESTful Endpoints:**
```typescript
// Goals
GET    /api/v1/roadmaps/:id/goals
POST   /api/v1/roadmaps/:id/goals
PUT    /api/v1/goals/:id
DELETE /api/v1/goals/:id

// Real-time Operations (WebSocket)
socket.emit('goal:move', {goalId, position})
socket.emit('solution:confidence', {solutionId, confidence})
socket.emit('decision:log', {entityId, decision})
```

**GraphQL Schema (Alternative):**
```graphql
type Goal {
  id: ID!
  title: String!
  why: String!
  solutions: [Solution!]!
  decisions: [Decision!]!
  position: Position!
}

type Mutation {
  createGoal(input: GoalInput!): Goal!
  updateGoalPosition(id: ID!, position: PositionInput!): Goal!
  logDecision(input: DecisionInput!): Decision!
}

type Subscription {
  goalUpdated(roadmapId: ID!): Goal!
  cursorMoved(roadmapId: ID!): CursorPosition!
}
```

### Security & Data Protection

**Security Measures:**
- **Encryption**: TLS 1.3 for transit, AES-256 for data at rest
- **XSS Prevention**: Content Security Policy, input sanitization
- **CSRF Protection**: Double-submit cookies
- **Rate Limiting**: 100 req/min per user, 1000 req/min per IP
- **SQL Injection**: Parameterized queries via Prisma
- **Dependency Scanning**: Automated via Dependabot
- **Secret Management**: AWS Secrets Manager for credentials

**Data Protection:**
- **GDPR Compliance**: Data export, right to deletion
- **Backup Strategy**: Daily automated backups, 30-day retention
- **Disaster Recovery**: Multi-region failover, RPO: 1hr, RTO: 4hrs
- **Data Retention**: Soft deletes with 30-day recovery window
- **Audit Logging**: All data modifications logged with user/timestamp

---

## Measuring Success

### Quantitative Metrics

We'll know we've succeeded when:

1. **Alignment improves**: Cross-functional alignment score increases 25% (quarterly survey)
2. **Decisions accelerate**: Time-to-decision drops 40% (decision log timestamps)
3. **Meetings shrink**: Strategy meetings are 30% shorter (calendar analysis)
4. **Adoption is broad**: 70% weekly active viewers (not just PM/leadership)
5. **Handoffs are clean**: 80% of Linear tickets include strategic context

### Qualitative Signals

Beyond numbers, we're looking for behavior changes:

- Teams reference the roadmap in Slack discussions (not just in meetings)
- Engineers check strategic context before starting work
- Stakeholders self-serve instead of asking "What's the status?"
- "Why are we building this?" has an immediate visual answer
- Decisions have rationales that survive team changes

### Tracking Implementation

Every interaction is instrumented:

```javascript
// Core events
track('goal.created', {stakeholder, phase, priority})
track('solution.confidence_changed', {from, to, goalId})
track('decision.logged', {entityType, fromState, toState})
track('zoom.performed', {fromLevel, toLevel, duration})
track('meeting.decision_accepted', {diffId, deciderId})
track('linear.handoff_clicked', {hasContext: true, decisionCount})
```

---

## Deployment & DevOps

### CI/CD Pipeline

**GitHub Actions Workflow:**
```yaml
# .github/workflows/deploy.yml
name: Deploy
on:
  push:
    branches: [main, develop]

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - run: npm ci
      - run: npm run lint
      - run: npm run type-check
      - run: npm test
      - run: npm run test:e2e

  deploy:
    needs: test
    runs-on: ubuntu-latest
    steps:
      - name: Build Docker image
      - name: Push to ECR
      - name: Deploy to ECS
      - name: Run smoke tests
```

**Deployment Environments:**
- **Development**: Auto-deploy from `develop` branch
- **Staging**: Auto-deploy from `main` with approval
- **Production**: Manual deploy with rollback capability

### Infrastructure as Code

```terraform
# terraform/main.tf
resource "aws_ecs_cluster" "roadmapper" {
  name = "roadmapper-cluster"
  
  setting {
    name  = "containerInsights"
    value = "enabled"
  }
}

resource "aws_rds_cluster" "postgres" {
  cluster_identifier = "roadmapper-db"
  engine            = "aurora-postgresql"
  engine_version    = "15.3"
  database_name     = "roadmapper"
  
  backup_retention_period = 7
  preferred_backup_window = "03:00-04:00"
}
```

### Monitoring & Observability

**Key Metrics:**
- API response time (p50, p95, p99)
- WebSocket connection count
- Canvas render performance (FPS)
- Database query performance
- Error rates by endpoint

**Alerting Thresholds:**
- API response time > 500ms (p95)
- Error rate > 1%
- Database CPU > 80%
- Memory usage > 85%
- Disk space < 10GB

## User Onboarding & Documentation

### First-Time User Experience

**Interactive Tutorial Flow:**
1. **Welcome Modal** - Value proposition and quick tour option
2. **Guided Goal Creation** - Interactive tooltip guides first goal
3. **Orbit Demonstration** - Animated demo of confidence levels
4. **Collaboration Intro** - Show real-time features
5. **Success Checkpoint** - Celebrate first complete roadmap

**Progressive Disclosure:**
- Basic features available immediately
- Advanced features unlock after 3 uses
- Power user shortcuts revealed through usage

### Help Documentation

**In-App Help:**
- Contextual tooltips on hover
- Command palette with search (Cmd+K)
- Video tutorials embedded in help panel
- Interactive demos for complex features

**Documentation Site:**
- Getting Started guide
- Video walkthroughs
- API documentation
- Best practices guide
- Template library

### User Feedback Loop

```typescript
// Feedback widget implementation
interface FeedbackWidget {
  trigger: 'frustration' | 'success' | 'manual'
  context: {
    feature: string
    action: string
    metadata: Record<string, any>
  }
  sentiment: 1 | 2 | 3 | 4 | 5
  comment?: string
}
```

## Risk Analysis & Mitigation

### Technical Risks

| Risk | Probability | Impact | Mitigation Strategy |
|------|------------|--------|-------------------|
| Canvas performance degradation | Medium | High | Implement virtualization, WebWorker offloading |
| Real-time sync conflicts | Medium | Medium | Use CRDT or OT, implement conflict resolution UI |
| Database scaling issues | Low | High | Read replicas, caching layer, query optimization |
| Browser compatibility | Low | Medium | Progressive enhancement, fallback rendering |
| Third-party API downtime | Medium | Low | Graceful degradation, queue retry logic |

### Business Risks

| Risk | Probability | Impact | Mitigation Strategy |
|------|------------|--------|-------------------|
| Low user adoption | Medium | High | User research, iterative feedback, onboarding optimization |
| Feature creep | High | Medium | Strict MVP scope, user validation gates |
| Competitor features | Medium | Medium | Unique value prop focus, fast iteration |
| Team expertise gaps | Low | Medium | Training, pair programming, external consultation |

### Security Risks

| Risk | Probability | Impact | Mitigation Strategy |
|------|------------|--------|-------------------|
| Data breach | Low | Critical | Encryption, security audits, pentesting |
| DDoS attacks | Low | High | CloudFlare, rate limiting, auto-scaling |
| Insider threats | Low | High | Audit logs, least privilege, MFA |
| Supply chain attacks | Medium | High | Dependency scanning, vendor assessment |

## Cost Estimation & Resource Planning

### MVP Costs (Weeks 1-3)

**Infrastructure (Monthly):**
- Vercel/Netlify hosting: $0 (free tier)
- Custom domain: $15/year
- **Total Infrastructure: ~$1.25/month**

**Services (Monthly):**
- Plausible Analytics: $9
- GitHub: $0 (public repo)
- **Total Services: ~$9/month**

**Team (Lean):**
- 1 Full-Stack Developer: 3 weeks
- 0.25 Designer: 1 week consultation
- **Total Team Cost: ~$15,000**

### Phase 4-5 Costs (If Validated)

**Added Infrastructure:**
- Railway/Heroku: $20/month
- PostgreSQL: $7/month
- **Total: ~$30/month**

**Added Services:**
- Sentry: $26/month
- SendGrid: $15/month
- **Total: ~$50/month**

### Phase 6+ Enterprise Costs

**Full Infrastructure (Monthly):**
- AWS ECS: $150
- RDS PostgreSQL: $200
- Redis: $50
- CloudFront: $50
- **Total: ~$450/month**

**Enterprise Services:**
- Auth0: $99/month
- DataDog: $150/month
- **Total: ~$250/month**

### Comparison: MVP vs Full Product

| Aspect | MVP (Week 1-3) | Full Product (Month 2+) |
|--------|---------------|------------------------|
| **Development Cost** | $15,000 | $92,500 |
| **Time to Market** | 3 weeks | 6-8 weeks |
| **Monthly Cost** | $10 | $700+ |
| **Team Size** | 1-2 people | 4-6 people |
| **Features** | Core roadmapping | Full collaboration |
| **Authentication** | None | SSO/SAML/MFA |
| **Storage** | Local only | Cloud + sync |
| **Break-even** | 10 users @ $99 | 100 teams @ $99 |

### ROI Projections (Revised)

**MVP Path:**
- Launch cost: $15,000
- Validate with 10 early adopters
- Charge $49/month initially
- Break-even: Month 6 (10 paying users)
- Decision point for Phase 4-6 investment

**Scale Path (If Validated):**
- Additional investment: $50,000
- Target: 100 teams @ $99/month  
- Break-even: Month 12
- Projected ARR Year 1: $60,000
- Projected ARR Year 2: $250,000

---

## Mobile & Responsive Strategy

### Mobile Approach

**Progressive Web App (PWA):**
- View-only mobile experience initially
- Touch gestures for pan and zoom
- Simplified UI with bottom navigation
- Offline viewing with Service Worker
- Native app shell with Capacitor (Phase 2)

**Responsive Breakpoints:**
```css
/* Tablet (768px-1024px) */
- Collapsible sidebar
- Touch-optimized controls
- Reduced information density

/* Mobile (< 768px) */
- Read-only canvas
- Simplified card views
- List view as default
- Quick actions menu
```

### Touch Interactions

```typescript
// Touch gesture handling
interface TouchGestures {
  pinch: 'zoom',
  swipe: 'pan',
  tap: 'select',
  longPress: 'contextMenu',
  doubleTap: 'focusZoom'
}
```

---

## Why This Matters

Recall Roadmapper isn't just another roadmapping tool. It's a fundamental shift in how we think about strategy:

**From feature lists to goal systems.** Every solution visually orbits a goal, making it impossible to lose sight of "why."

**From false precision to honest uncertainty.** Orbital distance makes confidence physical and visible.

**From information hiding to progressive disclosure.** The right details appear at the right zoom level.

**From forgotten decisions to preserved rationales.** Every state change captures the thinking behind it.

**From alignment theater to actual alignment.** Visual shared understanding replaces verbal interpretation.

This tool embodies a philosophy: strategy should be explorable, not just documentable. It should be a living space teams navigate together, not a static artifact one person maintains. By making abstract concepts like confidence and priority into physical properties like distance and size, we transform strategy from something we talk about into something we can see and touch.

The roadmap becomes a map—a real landscape teams can explore together, with landmarks they remember and paths they've traveled. That's the vision of Recall Roadmapper.

---

## Migration Strategy

### Import from Competitors

**Supported Import Sources:**
1. **Linear** - Direct API import of projects and issues
2. **Jira** - CSV export with field mapping
3. **ProductPlan** - JSON export format
4. **Airtable** - API integration
5. **Excel/CSV** - Template-based import

**Import Mapping:**
```typescript
interface ImportMapping {
  // Map external fields to our data model
  sourceField: string
  targetField: keyof Goal | keyof Solution
  transform?: (value: any) => any
  
  // Common transformations
  transformations: {
    dateFormat: (date: string) => Date
    priorityMapping: (priority: string) => 1 | 2 | 3
    confidenceMapping: (status: string) => number
  }
}
```

### Migration Wizard

**Step-by-step Process:**
1. **Source Selection** - Choose import source
2. **Authentication** - Connect to external tool
3. **Data Preview** - Review items to import
4. **Field Mapping** - Map fields with AI assistance
5. **Validation** - Check for conflicts/issues
6. **Import** - Progress bar with rollback option

### Data Export

**Export Formats:**
- **JSON** - Complete data with relationships
- **CSV** - Flat structure for spreadsheets
- **PDF** - Visual roadmap snapshot
- **PNG** - High-resolution image
- **Linear** - Push to Linear as projects

## Appendix: Detailed Specifications

### Version History

**Current Version: 5.0**
- v5.0 (Current) - Pivoted to MVP-first approach, deprioritized auth & complexity
- v4.0 - Added comprehensive technical implementation details
- v3.0 - Enhanced visual design and interaction patterns
- v2.0 - Added collaboration features
- v1.0 - Initial canvas concept

### Stakeholder Groups
The four stakeholder groups are (pending final confirmation):
1. **Free-to-Play (100%)** - Top of funnel users
2. **Staked Players (90%)** - Engaged participants  
3. **Curators (9%)** - Quality contributors and tastemakers
4. **Agent Developers (1%)** - Technical builders

### Performance Requirements
- Initial load: <2s for 100 nodes, <3.5s for 300 nodes
- Frame rate: ≥55fps during pan/zoom on modern hardware
- Transition animations: ≤150ms
- Uptime: 99.9% monthly SLA
- Concurrent editors: Support 10-20 simultaneous

### Accessibility
- WCAG AA compliance for color contrast
- Full keyboard navigation
- Screen reader support for critical paths
- Customizable color schemes for color blindness
- Text scaling without layout breaks

### Browser Support
- Chrome 90+ (primary)
- Firefox 88+
- Safari 14+
- Edge 90+
- No IE11 support

---

*End of Product Document v5.0*

**Summary of v5.0 Updates - MVP-First Approach:**

**Core Changes:**
- ✅ **Simplified to 3-week MVP** (was 6-8 weeks)
- ✅ **No authentication required** for MVP
- ✅ **No backend needed** initially (static site only)
- ✅ **Reduced cost from $92K to $15K**
- ✅ **Single developer** can build MVP (was 4-6 person team)

**Deprioritized to Post-MVP:**
- Authentication & authorization → Phase 6
- Real-time collaboration → Phase 6  
- Backend infrastructure → Phase 4
- Team management → Phase 6
- Linear integration → Phase 6
- Comments & @mentions → Phase 5

**MVP Focus (Weeks 1-3):**
1. **Week 1:** Core canvas with orbital physics
2. **Week 2:** Zoom, decision logging, export
3. **Week 3:** Polish and public launch

**Progressive Enhancement Path:**
- Phase 4: Add backend if users request persistence
- Phase 5: Add sharing if users request collaboration
- Phase 6: Add enterprise features for paying customers

**Key Benefits:**
- **Faster validation** of core concept
- **Lower risk** ($15K vs $92K)
- **User-driven development** based on actual usage
- **No technical debt** from premature optimization