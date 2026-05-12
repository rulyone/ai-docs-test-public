---
marp: true
theme: default
paginate: true
---

# Life

A visual essay on what it is, how it moves, and what it might mean.

---

## What we'll cover

- The arc — a life cycle, in shapes
- The stages — childhood to elder
- The engine — a single cell, working
- The question — what is it all *for*?

---

## The arc

```mermaid
flowchart LR
    Birth((Birth)) --> Growth[Growth]
    Growth --> Maturity[Maturity]
    Maturity --> Reproduction[Reproduction]
    Reproduction --> Aging[Aging]
    Aging --> Death(((Death)))
    Reproduction -. legacy .-> NextGen((Next generation))
    NextGen -. continues .-> Birth
```

A loop, not a line. Death feeds the next beginning.

---

## Stages of a life

```mermaid
flowchart TD
    A@{ shape: stadium, label: "Infancy 0–2" } --> B@{ shape: stadium, label: "Childhood 2–12" }
    B --> C@{ shape: stadium, label: "Adolescence 12–18" }
    C --> D@{ shape: stadium, label: "Young adulthood 18–35" }
    D --> E@{ shape: stadium, label: "Midlife 35–60" }
    E --> F@{ shape: stadium, label: "Elderhood 60+" }
    A:::start
    F:::endStage
    classDef start fill:#e8f4ff,stroke:#3b82f6,stroke-width:2px
    classDef endStage fill:#fef3c7,stroke:#d97706,stroke-width:2px
```

Each stage hands the next one a different question to answer.

---

## What each stage is *doing*

- **Infancy** — build the body, attach to caregivers
- **Childhood** — absorb language, world, rules
- **Adolescence** — separate, individuate, take risks
- **Young adult** — commit, build, mate, work
- **Midlife** — reassess, narrow, deepen
- **Elder** — integrate, transmit, let go

---

## Inside one cell

```mermaid
sequenceDiagram
    participant Env as Environment
    participant Mem as Cell membrane
    participant Mito as Mitochondrion
    participant Nuc as Nucleus
    participant Ribo as Ribosomes
    Env->>Mem: glucose + O2
    Mem->>Mito: nutrients in
    Mito->>Mito: cellular respiration
    Mito-->>Mem: ATP (energy)
    Nuc->>Ribo: mRNA transcript
    Ribo->>Ribo: synthesize protein
    Ribo-->>Mem: structural / functional proteins
    Mem->>Env: CO2 + H2O
    Note over Mito,Ribo: Repeats ~10^9 times per cell per day
```

A whole economy, running silently, in something smaller than a dust mote.

---

## The cellular cycle

```mermaid
flowchart LR
    G1[G1 grow] --> S[S copy DNA]
    S --> G2[G2 prep]
    G2 --> M[M divide]
    M --> G1
    M -. damage? .-> Apop[(Apoptosis)]
    G1 -. quiescent .-> G0[G0 rest]
    G0 -. resume .-> G1
```

Grow. Copy. Check. Divide. Or — quietly stop, if something is wrong.

---

## What is life *for*?

```mermaid
mindmap
  root((Meaning))
    Biological
      Survive
      Reproduce
      Pass on genes
    Relational
      Love
      Family
      Friendship
      Belonging
    Creative
      Make
      Build
      Express
      Leave a mark
    Transcendent
      Wonder
      Service
      Spirituality
      Connection to the whole
    Experiential
      Pleasure
      Beauty
      Curiosity
      Presence
```

No single answer. Multiple, layered, all real.

---

## A timeline of a human life

```mermaid
timeline
    title One life, in chapters
    section Becoming
        0 : First breath
        5 : First memories
        15 : First heartbreak
    section Building
        25 : First real choice
        35 : First reckoning
        45 : First loss of a parent
    section Distilling
        60 : First grandchild
        75 : First long silence
        90 : Last breath
```

The dates are placeholders. The shape is universal.

---

## Tensions we live inside

```mermaid
flowchart LR
    Self[Self] <--> Other[Other]
    Freedom[Freedom] <--> Belonging[Belonging]
    Stability[Stability] <--> Growth[Growth]
    Doing[Doing] <--> Being[Being]
    Self:::pole
    Other:::pole
    Freedom:::pole
    Belonging:::pole
    Stability:::pole
    Growth:::pole
    Doing:::pole
    Being:::pole
    classDef pole fill:#f9fafb,stroke:#6b7280,stroke-width:2px
```

A life is the ongoing negotiation between these poles. None of them "win."

---

## So what

- Life is a **cycle**, not a destination
- Stages are not goals — they are **vantage points**
- The engine is **cellular, relentless, miraculous**
- Meaning is **plural** — you don't pick one, you weave several
- The interesting question is not *what is life* but *what are you doing with this one*

---

## Closing

> "Tell me, what is it you plan to do
> with your one wild and precious life?"
> — Mary Oliver

Thanks.
