---
marp: true
theme: default
paginate: true
---

# Life in Diagrams

### Every Mermaid diagram type, applied to the human experience

---

## The Decision Tree of Being Born

*Flowchart — the branching logic that begins it all*

```mermaid
flowchart TD
    U((Universe)) -->|13.8 billion years| E[Earth forms]
    E --> EV[Evolution]
    EV --> H[Homo sapiens]
    H --> P{Parents meet?}
    P -->|Yes| C{Conception}
    P -->|No| NB[You never exist]
    C -->|Success| G[Gestation: 9 months]
    C -->|No| NB
    G --> B([You are born])
    B --> L[/Life begins\]
    L --> D{Every moment}
    D -->|Choose action| A[Act and shape your world]
    D -->|Hesitate| R[Regret lingers]
    A --> GR[Growth]
    R --> LE[Lesson learned]
    GR --> WS[Wisdom]
    LE --> WS
```

---

## First Words: A Sequence of Love

*Sequence diagram — the earliest exchange between parent and child*

```mermaid
sequenceDiagram
    actor Parent
    actor Infant
    actor World

    Parent->>Infant: You exist. Welcome.
    Infant-->>Parent: (cries)
    Parent->>Infant: You are safe. I am here.
    Infant-->>Parent: (quiets)
    World->>Infant: Gravity. Cold. Hunger.
    Infant->>Parent: (reaches out)
    Parent-->>Infant: I will always reach back.
    Note over Parent,Infant: This loop runs for a lifetime
    Infant->>World: (first smile)
    World-->>Infant: Everything responds
```

---

## The Taxonomy of a Person

*Class diagram — what we inherit, what we carry, what we pass on*

```mermaid
classDiagram
    class LivingBeing {
        +int age
        +String dna
        +breathe()
        +metabolize()
    }
    class Human {
        +String name
        +String language
        +String culture
        +dream()
        +regret()
        +create()
    }
    class Parent {
        +List children
        +String wisdomPassed
        +nurture()
        +letGo()
    }
    class Child {
        +String curiosity
        +float fearLevel
        +explore()
        +makeBelieves()
    }
    class Elder {
        +int memoriesCount
        +String legacy
        +reflect()
        +teach()
    }

    LivingBeing <|-- Human
    Human <|-- Parent
    Human <|-- Child
    Human <|-- Elder
    Parent "1" --> "*" Child : raises
    Child --> Elder : becomes
```

---

## States of the Human Mind

*State diagram — how consciousness cycles through its conditions*

```mermaid
stateDiagram-v2
    [*] --> Dreaming : birth / sleep

    Dreaming --> Awake : morning
    Awake --> Curious : wonder strikes
    Awake --> Anxious : uncertainty

    Curious --> Joyful : discovery
    Curious --> Confused : complexity

    Anxious --> Resilient : facing it
    Anxious --> Numb : avoidance

    Joyful --> Awake : moment passes
    Confused --> Curious : reframing
    Resilient --> Joyful : breakthrough

    Numb --> Grieving : thawing
    Grieving --> Healing : time + care
    Healing --> Awake : integration

    Awake --> Dreaming : night
    Dreaming --> [*] : death / peace
```

---

## The Relationships That Define Us

*ER diagram — the relational schema of a life*

```mermaid
erDiagram
    PERSON ||--o{ FRIENDSHIP : "forms"
    PERSON ||--o{ LOVE : "gives and receives"
    PERSON ||--|| SELF : "inhabits"
    PERSON }o--|| FAMILY : "born into"
    PERSON }o--o{ COMMUNITY : "belongs to"

    FRIENDSHIP {
        string shared_memory
        int years_known
        string trust_level
    }
    LOVE {
        string kind
        float intensity
        bool reciprocated
    }
    SELF {
        string core_values
        string inner_narrative
        string wounds
        string gifts
    }
    FAMILY {
        string name
        string traditions
        string unspoken_rules
    }
    COMMUNITY {
        string place
        string purpose
        int size
    }
```

---

## A Human Life: Project Plan

*Gantt chart — the schedule we never agreed to but live anyway*

```mermaid
gantt
    title The Unplanned Project: A Human Life
    dateFormat YYYY
    axisFormat %Y

    section Childhood
        Birth and survival         :done, c1, 0000, 5y
        Learning language          :done, c2, 0001, 6y
        School begins              :done, c3, 0005, 12y

    section Youth
        Identity search            :active, y1, 0013, 7y
        First heartbreak           :crit, y2, 0016, 2y
        Leaving home               :y3, 0018, 4y

    section Adulthood
        Building a life            :a1, 0022, 20y
        Raising others             :a2, 0028, 18y
        Career peak                :a3, 0035, 15y
        Midlife reckoning          :crit, a4, 0045, 5y

    section Wisdom Years
        Simplifying                :w1, 0055, 15y
        Letting go                 :w2, 0065, 10y
        Final chapter              :crit, w3, 0075, 10y
```

---

## How We Spend Our Days

*Pie chart — the honest accounting of a lifetime*

```mermaid
pie title How a Human Spends 80 Years
    "Sleep" : 26
    "Work" : 13
    "Screen time" : 11
    "Eating and drinking" : 4
    "Caring for others" : 6
    "Exercise and movement" : 3
    "Meaningful connection" : 7
    "Creativity and play" : 5
    "Worry" : 8
    "Everything else" : 17
```

---

## The Map of a Mind

*Mindmap — the universe inside one skull*

```mermaid
mindmap
  root((A Human Mind))
    Memory
      Childhood
        First fear
        First joy
      Lost moments
      Fabricated details
    Dreams
      Recurring nightmares
      Impossible wishes
      Unfinished futures
    Beliefs
      About self
        Worth
        Capability
      About others
        Trust
        Expectation
      About the world
        Fair or cruel
        Meaningful or random
    Creativity
      Language
      Music
      Movement
      Story
    Shadow
      Grief
      Shame
      Rage
      Longing
```

---

## Milestones of a Century

*Timeline — the arc from cradle to cosmos*

```mermaid
timeline
    title One Century of Human Life
    0 : Born : First breath
    2 : First words : First steps
    5 : School begins
    13 : Adolescence : Identity forms
    18 : Leaves home : Votes for first time
    25 : First major love : Career begins
    30 : Decade of building
    40 : Midpoint : Questioning everything
    50 : Wisdom accelerates : Body slows
    60 : Grandchildren perhaps : Legacy considered
    70 : Simplifying : Grateful for small things
    80 : Full circle : Stories told
    85 : Last great love : Final journey begins
```

---

## The Evolution of Self: A Git History

*GitGraph — branching, merging, and who we become*

```mermaid
gitGraph
    commit id: "Born (v0.1)"
    commit id: "Learn to walk"
    branch childhood
    checkout childhood
    commit id: "Curiosity peaks"
    commit id: "First best friend"
    checkout main
    merge childhood id: "Enter adolescence"
    branch identity-crisis
    checkout identity-crisis
    commit id: "Who am I?"
    commit id: "Experiment wildly"
    commit id: "Heartbreak"
    checkout main
    merge identity-crisis id: "Adult self emerges"
    branch relationships
    checkout relationships
    commit id: "Fall in love"
    commit id: "Build a home"
    checkout main
    branch loss
    checkout loss
    commit id: "Grief"
    commit id: "Rebuild"
    checkout main
    merge relationships id: "Family grows"
    merge loss id: "Wisdom earned"
    commit id: "Elder (v∞)"
```

---

## The Journey of a Human Day

*User Journey — the emotional score of Tuesday*

```mermaid
journey
    title The Emotional Journey of an Ordinary Day
    section Morning
        Wake before alarm: 2: Self
        First coffee: 5: Self
        Check phone: 3: Self, Anxiety
        Shower: 4: Self
    section Work
        Commute: 2: Self, Body
        Meaningful work: 4: Self, Colleagues
        Pointless meeting: 1: Self, Colleagues
        Lunch alone: 3: Self
    section Evening
        Call a parent: 4: Self, Family
        Cook dinner: 4: Self
        Watch something comforting: 3: Self
        Lie awake thinking: 2: Self, Mind
    section Night
        Finally sleep: 5: Self, Body
```

---

## Priorities vs. Time Spent

*Quadrant Chart — what matters vs. what gets our hours*

```mermaid
quadrantChart
    title What We Value vs. What We Actually Do
    x-axis Low Time Spent --> High Time Spent
    y-axis Low Importance --> High Importance
    quadrant-1 Sacred and protected
    quadrant-2 Meaningful but neglected
    quadrant-3 Low value low time
    quadrant-4 Busyness trap
    Deep relationships: [0.25, 0.95]
    Creative work: [0.20, 0.85]
    Rest and sleep: [0.45, 0.80]
    Exercise: [0.15, 0.75]
    Email and messages: [0.75, 0.30]
    Social media: [0.80, 0.15]
    Commuting: [0.60, 0.20]
    Meetings: [0.65, 0.35]
    Learning: [0.30, 0.70]
    News consumption: [0.55, 0.25]
```

---

## The Requirements of a Good Life

*Requirement Diagram — what a meaningful life demands*

```mermaid
requirementDiagram

    requirement meaning {
        id: 1
        text: Life must feel purposeful
        risk: High
        verifymethod: Inspection
    }

    requirement connection {
        id: 2
        text: Genuine bonds with others
        risk: High
        verifymethod: Demonstration
    }

    requirement growth {
        id: 3
        text: Continuous learning and change
        risk: Medium
        verifymethod: Analysis
    }

    requirement acceptance {
        id: 4
        text: Peace with what cannot change
        risk: High
        verifymethod: Inspection
    }

    element daily_practice {
        type: practice
        docref: the examined life
    }

    element community {
        type: environment
        docref: belonging
    }

    daily_practice - satisfies -> meaning
    daily_practice - satisfies -> growth
    community - satisfies -> connection
    acceptance - refines -> meaning
```

---

## Energy: How Life Flows Through the World

*Sankey diagram — the flow of vitality across living systems*

```mermaid
---
config:
  sankey:
    showValues: false
---
sankey

Sun,Plants,100
Plants,Herbivores,40
Plants,Soil,30
Plants,Atmosphere,30
Herbivores,Carnivores,15
Herbivores,Soil,15
Herbivores,Heat,10
Carnivores,Apex Predators,5
Carnivores,Soil,5
Carnivores,Heat,5
Apex Predators,Soil,3
Apex Predators,Heat,2
Soil,New Life,48
Soil,Atmosphere,5
```

---

## Vitality Across the Lifespan

*XY Chart — the physical and emotional arc of a life*

```mermaid
xychart
    title "Human Vitality Across the Decades"
    x-axis ["10s", "20s", "30s", "40s", "50s", "60s", "70s", "80s"]
    y-axis "Vitality Score (0-100)" 0 --> 100
    bar [70, 95, 88, 75, 65, 58, 45, 35]
    line [45, 55, 62, 70, 75, 78, 80, 82]
```

*Bars: physical energy. Line: wisdom and inner peace.*

---

## The Architecture of a Life

*Block diagram — the systems that hold us together*

```mermaid
block-beta
    columns 3

    block:core:1
        columns 1
        identity["Identity"]
        values["Values"]
        purpose["Purpose"]
    end

    block:social:1
        columns 1
        family["Family"]
        friends["Friends"]
        community["Community"]
        work["Work"]
    end

    block:care:1
        columns 1
        body["Body"]
        mind["Mind"]
        spirit["Spirit"]
        rest["Rest"]
    end

    core --> social
    core --> care
    social --> care
```

---

## The End Is Also a Beginning

*Flowchart — what happens to a life after it is lived*

```mermaid
flowchart TD
    L([Life]) --> D{Death}
    D --> M[Memories in others]
    D --> W[Works left behind]
    D --> G[Genes carried forward]
    D --> E[Energy returned to Earth]

    M --> S[Stories told]
    W --> I[Ideas that outlive you]
    G --> C[Children, grandchildren]
    E --> N[New life]

    S --> L2([Future lives changed])
    I --> L2
    C --> L2
    N --> L2

    L2 -->|the cycle continues| L3((Life))
```

---

# Thank You

Life is not a problem to be solved.
It is a diagram to be drawn — imperfectly, beautifully, together.

*Every chart type tells a different truth about the same mystery.*
