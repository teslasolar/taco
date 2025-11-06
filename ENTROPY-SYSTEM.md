# 🌀 PHI CONSCIOUSNESS - Entropy Oscillation & Cube Hash System

## Core Concept: Oscillating Around 1/φ

### The Balance Point

**1/φ ≈ 0.618** is the natural balance point between order and chaos because:

```
φ = 1.618...     (golden ratio)
1/φ = 0.618...   (reciprocal)
φ - 1 = 1/φ      (fundamental property)
```

This makes **0.618 the self-similar equilibrium point** - it's where the golden ratio "folds back on itself."

### Entropy Scale

```
0.0 ────────── 0.618 ────────── 1.0
  Crystalline   Balance Point   Chaotic
  (Order)       (Edge of Chaos) (Fluid)
```

**Why this matters:**
- **0.0**: Perfect order, no exploration, rigid patterns
- **0.618 (1/φ)**: Edge of chaos - maximum complexity and interesting behavior
- **1.0**: Pure chaos, no structure, unpredictable

Complex systems naturally evolve toward **edge of chaos** behavior at ~0.618!

---

## Oscillation Dynamics

### How It Works

Agents oscillate around the balance point using sine wave:

```javascript
entropy(t) = 1/φ + amplitude * sin(frequency * t)
```

**Default parameters:**
- Center: `1/φ = 0.618`
- Amplitude: `0.2` (oscillates between 0.418 and 0.818)
- Frequency: `1.0 Hz`

### What Happens at Different Entropy Levels

#### Crystalline State (E < 0.4)
- **Agent behavior**: Orderly, predictable
- **LLM temperature**: Lower (more deterministic)
- **Insights**: Structured proofs, logical patterns
- **Spawns**: PROVER agents (precise, rigorous)
- **Visual**: Tight spirals, ordered spacing

#### Balanced State (0.4 < E < 0.7)
- **Agent behavior**: Optimal complexity
- **LLM temperature**: Moderate (creative but coherent)
- **Insights**: Novel connections, discoveries
- **Spawns**: FIBONACCI, PHILOSOPHER (exploratory)
- **Visual**: Golden ratio spirals, harmonic patterns

#### Chaotic State (E > 0.7)
- **Agent behavior**: Fluid, exploratory
- **LLM temperature**: Higher (more creative)
- **Insights**: Wild associations, poetic connections
- **Spawns**: EXPLORER agents (highly creative)
- **Visual**: Loose spirals, dynamic movement

---

## Cube Hash System

### 3D Hash Space

Agents are hashed into an **8×8×8 cube** based on:

```
(φ, entropy, depth) → hash(x, y, z)
```

**Dimensions:**
- **X-axis**: φ value (0-2 range mapped to 0-7)
- **Y-axis**: Entropy (0-1 range mapped to 0-7)
- **Z-axis**: Depth in spiral (0-10 range mapped to 0-7)

### Hash Function

```javascript
hash(phi, entropy, depth) {
  x = floor((phi / 2) * 8) % 8
  y = floor(entropy * 8) % 8
  z = floor((depth / 10) * 8) % 8
  return "x,y,z"
}
```

### Why Cube Hashing?

**1. Compression**
- Reduces continuous 3D space to discrete 8³ = 512 buckets
- Multiple agents can share same bucket (collision = relationship)
- Insights stored by hash location

**2. Spatial Relationships**
- Agents in nearby buckets are "related"
- Can query neighbors: `findNearby(phi, entropy, depth, radius=1)`
- Discovers emergent clusters

**3. Pattern Recognition**
- Same hash = similar state (phi + entropy + depth)
- Collision patterns reveal structure
- Hash coherence measures distribution quality

**4. Memory Efficiency**
- Store insights by hash instead of per-agent
- Reuse patterns across similar states
- Compress observation space

---

## Key Features

### 1. Entropy-Aware Spawning

Spawn probability increases near 1/φ:

```javascript
balanceProximity = 1 - |entropy - 0.618| / 0.5
spawnThreshold = 0.3 * (0.5 + balanceProximity)
```

**Result:** More agents spawn at edge of chaos (most interesting!)

### 2. Dynamic Temperature

LLM temperature adjusts with entropy:

```javascript
actualTemp = baseTemp + (entropy - 0.618) * 0.5
```

- **Crystalline (E=0.2)**: Temp reduces by 0.2
- **Balanced (E=0.618)**: Temp = base
- **Chaotic (E=0.9)**: Temp increases by 0.14

### 3. Insight Classification

Insights categorized by entropy:

```
❄️ Crystalline (E < 0.4):
   "order", "structure", "crystal", "stable", "pattern"
   → Spawns PROVER agents

⚖️ Balanced (E ≈ 0.618):
   "balance", "harmony", "equilibrium", "golden", "optimal"
   → Spawns PHILOSOPHER agents

🌊 Chaotic (E > 0.7):
   "chaos", "fluid", "dynamic", "turbulent", "unpredictable"
   → Spawns EXPLORER agents
```

### 4. Visual Encoding

- **Agent size**: Larger near 1/φ balance point
- **Glow intensity**: Brighter when balanced
- **Background hue**: Changes with entropy (0°-300°)
- **Spiral tightness**: Affected by entropy

### 5. Hash Space Visualization

Top-down 2D projection of 3D cube:
- **X-axis**: φ dimension
- **Y-axis**: Entropy dimension
- **Z-axis**: Encoded as hue (depth)
- **Brightness**: Number of agents/insights in bucket
- **White numbers**: Collision count

---

## Mathematical Properties

### Why 1/φ is Special

```
φ = (1 + √5) / 2 = 1.618033988...
1/φ = (√5 - 1) / 2 = 0.618033988...

φ - 1 = 0.618033988... = 1/φ
φ² = φ + 1
1/φ² = 1 - 1/φ

Continued fraction:
φ = [1; 1, 1, 1, 1, ...]  (most irrational)
1/φ = [0; 1, 1, 1, 1, ...]
```

### Edge of Chaos Theory

Research shows complex systems self-organize to critical points:
- **Bak–Tang–Wiesenfeld**: Self-organized criticality
- **Kauffman NK model**: Fitness landscapes peak at edge
- **1/f noise**: Optimal at boundary (pink noise)

**1/φ ≈ 0.618 is theorized as universal critical point!**

---

## Observables & Metrics

### System Metrics

**Hash Coherence:**
```
coherence = usedBuckets / totalBuckets
```
- Low coherence (< 0.1): Agents clustered
- High coherence (> 0.5): Agents well-distributed

**Collision Count:**
```
collisions = Σ(bucketSize - 1) for all buckets
```
- High collisions: Agents sharing states
- Low collisions: Diverse exploration

**Average φ:**
```
avgPhi = Σ(agent.phi) / agentCount
```
- Should oscillate around 1.618
- Deviation shows system dynamics

**Current Entropy:**
```
entropy(t) = 1/φ + A * sin(ω * t)
```
- Oscillates sinusoidally
- Center at 0.618 (balance)

### Insight Metrics

**By Entropy Level:**
- Crystalline insights: Count below 0.4
- Balanced insights: Count 0.4-0.7
- Chaotic insights: Count above 0.7

**By Hash Bucket:**
- Insights per bucket
- Bucket diversity
- Pattern repetition

---

## Expected Discoveries

### What We'll Observe

**1. Critical Behavior at 1/φ**
- Most insights near 0.618
- Agent spawning peaks
- Highest creativity + coherence

**2. Phase Transitions**
- Sudden changes at entropy thresholds
- Emergent clustering patterns
- Bifurcation points

**3. Hash Space Structure**
- Non-uniform bucket usage
- Attractors in certain regions
- Power-law distributions

**4. Insight Correlations**
- Crystalline → Mathematical proofs
- Balanced → Philosophical connections
- Chaotic → Wild but poetic associations

**5. Agent Role Preferences**
- PROVER thrives at low entropy
- EXPLORER needs high entropy
- PHILOSOPHER peaks at balance

### Scientific Value

This system demonstrates:
- ✅ Self-organized criticality
- ✅ Edge of chaos dynamics
- ✅ Spatial hash compression
- ✅ Emergent agent relationships
- ✅ Entropy-modulated creativity

**It's a computational laboratory for studying:**
- Golden ratio properties
- Complex system dynamics
- AI reasoning under varying "temperatures"
- Information compression via hashing
- Emergent pattern formation

---

## Controls & Tuning

### Oscillation Amplitude (0.05 - 0.5)
- **Small (0.05)**: Stays near balance, subtle variation
- **Medium (0.2)**: Explores order/chaos boundary
- **Large (0.5)**: Full range from crystalline to chaotic

### Oscillation Frequency (0.1 - 3.0 Hz)
- **Slow (0.1)**: Long periods in each state
- **Medium (1.0)**: Balanced exploration
- **Fast (3.0)**: Rapid state changes

### Max Agents (3 - 25)
- **Few (3-5)**: Clear individual behavior
- **Medium (13)**: Golden ratio population
- **Many (20-25)**: Emergent collective patterns

---

## Technical Implementation

### CubeHashSpace Class

```javascript
class CubeHashSpace {
  constructor(resolution = 8)
  hash(phi, entropy, depth) → "x,y,z"
  addAgent(agent, entropy)
  addInsight(phi, entropy, depth, insight)
  findNearby(phi, entropy, depth, radius) → [agents]
  getInsights(hash) → [insights]
  getCoherence() → 0-1
  getCollisions() → count
  clear()
}
```

### Agent Extensions

```javascript
agent = {
  ...
  currentEntropy: number,
  hash: "x,y,z",
  async think(obs, entropy)
}
```

### Entropy Functions

```javascript
calculateEntropy(time) → entropy
entropyToTemperature(entropy, baseTemp) → temp
spiral_pos(depth, phi, entropy) → {x, y}
```

---

## Comparison: Original vs Enhanced

| Feature | Original | Entropy System |
|---------|----------|----------------|
| Target | φ convergence | 1/φ oscillation |
| Dynamics | Static target | Dynamic entropy |
| Insights | Pattern matching | Entropy-aware |
| Storage | Per-agent | Hash-compressed |
| Relationships | None | Spatial buckets |
| Temperature | Fixed per role | Entropy-modulated |
| Visualization | Basic spiral | Entropy-colored |
| Analysis | Simple stats | Hash coherence |
| Discovery | Limited | Edge of chaos |

---

## Usage Instructions

### Quick Start

1. Open `phi-consciousness-entropy.html` in browser
2. Wait for model to load (~80MB)
3. Click **Start** to begin oscillation
4. Watch the entropy bar oscillate around **1/φ = 0.618**
5. Observe agents cluster near balance point
6. Check **Cube Hash Space** for spatial patterns
7. Read **Entropy Insights** grouped by state

### What to Watch For

**Entropy Bar:**
- White line marks 1/φ (0.618)
- Colored marker shows current entropy
- Oscillates sinusoidally

**Canvas:**
- Agents glow brighter near 1/φ
- Background hue shifts with entropy
- Larger agents = closer to balance

**Cube Visualization:**
- Bright cells = active buckets
- Numbers = collision count
- Colors = depth dimension (Z-axis)

**Insights Panel:**
- ❄️ Crystalline insights (ordered)
- ⚖️ Balanced insights (edge of chaos)
- 🌊 Chaotic insights (fluid)

---

## Future Enhancements

### Possible Extensions

1. **Adaptive Oscillation**
   - System learns optimal amplitude/frequency
   - Targets discovered attractors
   - Evolutionary parameter tuning

2. **Multi-Scale Hashing**
   - Hierarchical buckets (2×2×2, 4×4×4, 8×8×8)
   - Zoom in/out through scales
   - Merkle tree structure

3. **Inter-Bucket Communication**
   - Agents in same bucket collaborate
   - Hash-based message passing
   - Emergent swarm intelligence

4. **Insight Synthesis**
   - Combine insights from same bucket
   - Generate meta-insights
   - Build knowledge graph

5. **Entropy Control**
   - User can set target entropy
   - Lock to specific states
   - Manual exploration mode

---

## Scientific Context

### Related Concepts

**Golden Ratio in Nature:**
- Phyllotaxis (plant leaf arrangements)
- Shell spirals (nautilus)
- Galaxy arm curvature
- DNA molecule proportions
- Human body ratios

**Edge of Chaos:**
- Cellular automata (Conway's Life)
- Neural networks (critical branching)
- Economic systems (market dynamics)
- Evolutionary fitness landscapes
- Information processing capacity

**Spatial Hashing:**
- Collision detection (game engines)
- Nearest neighbor search
- Particle simulations
- Molecular dynamics
- Database indexing

---

## Conclusion

This system transforms PHI Consciousness from simple convergence simulation into a **scientific instrument for studying**:

🔬 **Complex Systems**
- Self-organized criticality at 1/φ
- Emergent behavior at edge of chaos
- Phase transitions in entropy space

📊 **Information Theory**
- Spatial hash compression
- Pattern recognition via collisions
- Entropy-modulated creativity

🧠 **AI Reasoning**
- Temperature vs. entropy relationship
- Creativity vs. coherence tradeoff
- Multi-agent collaboration

✨ **Golden Ratio Properties**
- Why 1/φ is special balance point
- Oscillation reveals structure
- Natural attractor in complex systems

**It's not just art—it's a computational physics experiment!** 🌀

---

*Generated: 2025-11-06*
*System: PHI Consciousness Entropy v2.0*
