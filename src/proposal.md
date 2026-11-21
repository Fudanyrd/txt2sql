---
marp: true
paginate: true
theme: default
style: |
  section {
    background-color: #f7fbff;
    color: #0b2545;
    font-size: 21px;
    padding: 44px 52px;
  }
  section::after {
    color: #5b7c99;
    font-size: 14px;
  }
  section h1 {
    font-size: 48px;
    font-weight: bold;
    text-align: center;
    padding: 20px 30px;
    color: white;
    background-color: #3333ab;
    border-radius: 8px;
  }
  section h2 {
    font-size: 33px;
    font-weight: bold;
    text-align: left;
    margin: 0 0 20px;
    padding: 12px 18px;
    border-radius: 8px;
    background: linear-gradient(90deg, #0d3b66, #1565c0);
    color: #ffffff;
  }
  .hero {
    text-align: center;
    padding-top: 90px;
  }
  .kicker {
    color: #0f766e;
    font-size: 17px;
    font-weight: 700;
    letter-spacing: 2px;
    text-transform: uppercase;
  }
  .title {
    margin: 18px auto 12px;
    padding: 18px 24px;
    border-radius: 12px;
    background: linear-gradient(135deg, #0d3b66, #1565c0 60%, #0891b2);
    color: #ffffff;
    font-size: 46px;
    font-weight: bold;
  }
  .subtitle {
    color: #335c7d;
    font-size: 23px;
    line-height: 1.35;
  }
  .author {
    margin-top: 26px;
    color: #0d3b66;
    font-size: 27px;
  }
  .author span {
    display: block;
    margin-top: 6px;
    color: #5b7c99;
    font-size: 16px;
    font-weight: normal;
  }
  .definition {
    background-color: #e6f0fa;
    border-left: 6px solid #1565c0;
    border-radius: 8px;
    padding: 14px 20px;
    font-size: 21px;
    line-height: 1.35;
  }
  .definition strong {
    color: #0d3b66;
  }
  .example {
    display: grid;
    grid-template-columns: 1fr auto 1fr;
    gap: 14px;
    align-items: stretch;
    margin-top: 16px;
  }
  .panel {
    background-color: #ffffff;
    border: 1px solid #cfe0f0;
    border-radius: 10px;
    padding: 14px 18px;
    box-shadow: 0 2px 6px rgba(13, 59, 102, 0.08);
  }
  .panel .label {
    display: block;
    margin-bottom: 7px;
    color: #5b7c99;
    font-size: 13px;
    font-weight: 700;
    letter-spacing: 1px;
    text-transform: uppercase;
  }
  .panel p {
    margin: 0;
    font-size: 18px;
    line-height: 1.4;
  }
  .panel code {
    color: #0d3b66;
    font-size: 17px;
  }
  .nl {
    background-color: #e8f5f1;
    border-color: #a7d8c9;
  }
  .sql {
    background-color: #e8f1fb;
    border-color: #a9c8ea;
  }
  .arrow {
    display: flex;
    align-items: center;
    justify-content: center;
    color: #1565c0;
    font-size: 34px;
    font-weight: bold;
  }
  .pipeline {
    display: grid;
    grid-template-columns: repeat(4, minmax(0, 1fr));
    gap: 12px;
    margin-top: 16px;
  }
  .step {
    background-color: #ffffff;
    border-top: 5px solid #0891b2;
    border-radius: 8px;
    padding: 10px 14px;
    font-size: 16px;
    line-height: 1.35;
    box-shadow: 0 2px 6px rgba(13, 59, 102, 0.07);
  }
  .step b {
    display: block;
    margin-bottom: 3px;
    color: #0d3b66;
    font-size: 18px;
  }
  .card-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 14px;
    margin-top: 14px;
  }
  .card {
    background-color: #ffffff;
    border: 1px solid #cfe0f0;
    border-radius: 10px;
    padding: 14px 16px;
    box-shadow: 0 2px 6px rgba(13, 59, 102, 0.08);
  }
  .card h3 {
    margin: 0 0 7px;
    color: #0d3b66;
    font-size: 19px;
  }
  .card p {
    margin: 0;
    font-size: 16px;
    line-height: 1.38;
  }
  .badge {
    display: inline-block;
    margin-bottom: 8px;
    padding: 2px 9px;
    border-radius: 999px;
    background-color: #1565c0;
    color: #ffffff;
    font-size: 13px;
    font-weight: 700;
  }
  .badge.teal {
    background-color: #0f766e;
  }
  .badge.green {
    background-color: #2e7d32;
  }
  .chips {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-top: 14px;
  }
  .chip {
    padding: 5px 12px;
    border: 1px solid #a9c8ea;
    border-radius: 999px;
    background-color: #e6f0fa;
    color: #0d3b66;
    font-size: 15px;
    font-weight: 600;
  }
  .evolution {
    display: grid;
    grid-template-columns: repeat(4, minmax(0, 1fr));
    gap: 10px;
    margin-top: 14px;
  }
  .era {
    padding: 8px 12px;
    border-left: 4px solid #0f766e;
    border-radius: 6px;
    background-color: #eef7f4;
    color: #335c7d;
    font-size: 14px;
    line-height: 1.3;
  }
  .era b {
    display: block;
    color: #0d3b66;
    font-size: 15px;
  }
  .takeaway {
    margin-top: 14px;
    padding: 11px 18px;
    border-radius: 8px;
    background-color: #0d3b66;
    color: #e8f1fb;
    font-size: 17px;
    line-height: 1.35;
  }
  .takeaway strong {
    color: #ffffff;
  }
  .sources {
    margin-top: 16px;
    padding-top: 7px;
    border-top: 1px solid #cfe0f0;
    color: #5b7c99;
    font-size: 12.5px;
    line-height: 1.35;
  }
  .sources b {
    color: #335c7d;
  }
  section table {
    width: 100%;
    margin-top: 10px;
    border-collapse: collapse;
    font-size: 16.5px;
  }
  section thead th {
    padding: 8px 10px;
    background-color: #0d3b66;
    color: #ffffff;
    text-align: left;
  }
  section tbody td {
    padding: 7px 10px;
    border-bottom: 1px solid #cfe0f0;
    vertical-align: top;
    line-height: 1.32;
  }
  section tbody tr:nth-child(even) {
    background-color: #eef4fb;
  }
  section tbody tr:last-child td {
    border-top: 2px solid #0d3b66;
    font-weight: 700;
  }
  .trend {
    margin-top: 8px;
  }
  .plot {
    display: grid;
    grid-template-columns: repeat(6, minmax(0, 1fr));
    align-items: end;
    height: 218px;
    padding: 0 8px;
    border-bottom: 2px solid #8fb3d1;
  }
  .bcol {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-end;
    height: 100%;
  }
  .bcount {
    margin-bottom: 3px;
    color: #0d3b66;
    font-size: 14px;
    font-weight: 700;
  }
  .stack {
    display: flex;
    flex-direction: column-reverse;
    width: 56px;
    overflow: hidden;
    border-radius: 4px 4px 0 0;
  }
  .seg {
    width: 100%;
  }
  .seg.bench { background-color: #1565c0; }
  .seg.schema { background-color: #2e7d32; }
  .seg.llm { background-color: #ef6c00; }
  .seg.agentic { background-color: #00838f; }
  .seg.rank { background-color: #6a1b9a; }
  .seg.slm { background-color: #c62828; }
  .seg.ind { background-color: #546e7a; }
  .years {
    display: grid;
    grid-template-columns: repeat(6, minmax(0, 1fr));
    padding: 4px 8px 0;
    color: #335c7d;
    font-size: 14px;
    font-weight: 600;
    text-align: center;
  }
  .chart-legend {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 6px 16px;
    margin-top: 9px;
    color: #335c7d;
    font-size: 12.5px;
  }
  .chart-legend span {
    display: inline-flex;
    align-items: center;
    gap: 5px;
  }
  .dot {
    display: inline-block;
    width: 10px;
    height: 10px;
    border-radius: 2px;
  }
  .findings {
    margin: 11px 0 0;
    padding-left: 20px;
    font-size: 16.5px;
    line-height: 1.38;
  }
  .findings li {
    margin-bottom: 3px;
  }
---

<div class="hero">

<div class="kicker">Natural Language × Relational Data</div>

<!-- FIXME: -->
<div class="title">
Research Proposal for a Text-to-SQL Method
</div>

<div class="author">
Anonymous
</div>

</div>

---

<h1>Introduction to Text-to-SQL</h1>

---

## What is Text-to-SQL?

<div class="definition">
<strong>Text-to-SQL</strong> (also <strong>NL-to-SQL</strong>) translates a natural-language question, together with a database schema, into an <strong>executable SQL query</strong>. It sits at the core of natural-language interfaces for databases and lowers the barrier to structured data access.
</div>

<div class="example">

<div class="panel nl">
<span class="label">Natural language</span>
<p>“What is the average salary of employees in the sales department?”</p>
</div>

<div class="arrow">→</div>

<div class="panel sql">
<span class="label">Executable SQL</span>
<p><code>SELECT AVG(salary)<br />FROM employees<br />WHERE department = 'sales';</code></p>
</div>

</div>

<div class="pipeline">
  <div class="step"><b>1 · Understand</b>Extract tables, columns, predicates, aggregations, and sort orders from the question.</div>
  <div class="step"><b>2 · Link</b>Ground question phrases in schema elements, database values, and join paths.</div>
  <div class="step"><b>3 · Translate</b>Build SQL that satisfies syntax and logical constraints.</div>
  <div class="step"><b>4 · Verify</b>Check execution and confirm the result matches user intent.</div>
</div>

<div class="takeaway">
<strong>Not just a translation task.</strong> Modern Text-to-SQL is an execution-aware semantic parsing and program-synthesis problem.
</div>

<div class="sources">
<b>Sources:</b> Liu et al., “A systematic review of natural language interfaces for databases,” Frontiers of Computer Science, 2026 (definition, two-stage NLU/NLT view, worked example). Choi et al., “Text-to-SQL in the Era of Large Language Models,” Electronics, 2026 (execution-aware parsing, grounding, verification).
</div>

---

## Why It Matters for Practitioners

<div class="card-grid">

<div class="card">
<span class="badge teal">Access</span>
<h3>Lower the barrier</h3>
<p>Non-experts retrieve structured information in natural language instead of learning schemas, joins, and SQL syntax.</p>
</div>

<div class="card">
<span class="badge">Productivity</span>
<h3>Faster insight</h3>
<p>Analysts and business users can move from question to query to answer without a hand-written query for every need.</p>
</div>

<div class="card">
<span class="badge green">Reach</span>
<h3>Embedded everywhere</h3>
<p>Powers business intelligence, structured web search, customer-support querying, intelligent QA, and low-code tools.</p>
</div>

</div>

<div class="chips">
  <div class="chip">Self-service analytics</div>
  <div class="chip">Enterprise data services</div>
  <div class="chip">Low-code development</div>
  <div class="chip">Conversational assistants</div>
</div>

<div class="evolution">
  <div class="era"><b>Rule-based</b>Precise but brittle; high maintenance.</div>
  <div class="era"><b>Neural / PLM</b>Learned parsing; needs task-specific data.</div>
  <div class="era"><b>LLM prompting</b>Few-shot and zero-shot SQL synthesis.</div>
  <div class="era"><b>Agentic systems</b>Retrieval, verification, and execution feedback.</div>
</div>

<div class="takeaway">
<strong>Why now:</strong> LLMs make zero-shot and few-shot SQL synthesis feasible, shifting research from hand-built parsers to system-level pipelines.
</div>

<div class="sources">
<b>Sources:</b> Liu et al. (2026) — barrier reduction, application areas, and the rule-based → ML → PLM → LLM evolution. Choi et al. (2026) — the shift toward LLM-based and agentic systems, and deployment concerns beyond accuracy.
</div>

---

## Challenges That Remain

<div class="card-grid">

<div class="card">
<span class="badge">Grounding</span>
<h3>Connect language to schema</h3>
<p>Systems must identify relevant tables and columns, ground phrases in database values, and infer valid join paths before writing SQL.</p>
</div>

<div class="card">
<span class="badge">Scale</span>
<h3>Large schemas</h3>
<p>Real databases can be too large for a prompt; the full schema adds context length, inference cost, and irrelevant information.</p>
</div>

<div class="card">
<span class="badge">Correctness</span>
<h3>Executable ≠ correct</h3>
<p>A query may run successfully yet return a result that differs from what the user intended, so execution-guided validation is needed.</p>
</div>

<div class="card">
<span class="badge teal">Efficiency</span>
<h3>Cost and stability</h3>
<p>LLM-based methods face output instability, limited semantic control, and high inference cost, with accuracy–cost trade-offs.</p>
</div>

<div class="card">
<span class="badge teal">Ambiguity</span>
<h3>Language vs. SQL</h3>
<p>Natural language is ambiguous and variable, while SQL demands precise semantic alignment and strict logical constraints.</p>
</div>

<div class="card">
<span class="badge green">Security</span>
<h3>Safety and privacy</h3>
<p>Valid queries can expose restricted data, modify data, or overload the database; prompt injection and jailbreaking add risk.</p>
</div>

</div>

<div class="takeaway">
<strong>The hard part is reliability, not syntax.</strong> Practical systems must jointly optimize grounding, semantic correctness, cost, and safety.
</div>

<div class="sources">
<b>Sources:</b> Choi et al. (2026) — schema/value grounding, large-schema context costs, semantic correctness, and security/safety risks. Liu et al. (2026) — ambiguity and variability of natural language, strict SQL constraints, output instability, and inference cost.
</div>

---

<h1>Literature Review</h1>

---

## Methodology of the Literature Review

<div class="card-grid">

<div class="card">
<span class="badge">1 · Seed</span>
<h3>Start from 6 seed papers</h3>
<p>Course-provided seeds: Purple (2024), MetaSQL (2024), GAR (2023), Combining SLM+LLM (2024), CATSQL (2023), Athena++ (2020).</p>
</div>

<div class="card">
<span class="badge teal">2 · Snowball</span>
<h3>Backward & forward search</h3>
<p>Walk each seed's references (backward) and the papers that cite it (forward) to grow the corpus.</p>
</div>

<div class="card">
<span class="badge green">3 · Classify</span>
<h3>Group by research front</h3>
<p>Screen the expanded set and assign every paper to one of seven research fronts.</p>
</div>

</div>

<div class="chips">
  <div class="chip">6 seed papers</div>
  <div class="chip">+ 27 via snowballing</div>
  <div class="chip">= 33 papers</div>
  <div class="chip">7 research fronts</div>
</div>

<div class="takeaway">
<strong>Result:</strong> snowballing turned 6 seeds into a 33-paper, 7-front map — 21 of the 27 added papers (78%) are from 2024 or later, keeping both pre-LLM anchors and the current LLM frontier.
</div>

<div class="sources">
<b>Sources:</b> <code>src/main.tex</code> — seed set, backward/forward snowballing, the 33-paper composition summary, and the research-front classification.
</div>

---

## Comparison of Different Schemes

Schemes and research fronts form a one-to-one mapping.

| Scheme | Core idea | # Publications |
|:--|:--|:--:|
| Benchmarks & evaluation | Curate datasets and execution-based metrics that probe realistic Text-to-SQL understanding. | 4 |
| Schema linking & neural parsing | Map question mentions to tables and columns inside neural encoder–decoder SQL parsers. | 6 |
| LLM prompting / decomposition | Break questions into sub-tasks and guide LLMs with staged prompts and in-context examples. | 10 |
| Agentic LLM (multi-agent) | Coordinate specialized LLM agents for schema retrieval, query generation, and iterative repair. | 5 |
| Generate-then-rank & self-correction | Sample multiple candidate SQL queries, then rank, select, or repair them using execution feedback. | 4 |
| SLM–LLM collaboration & open-source | Pair small and large models, or release open models, to trade accuracy against inference cost. | 3 |
| Industrial NLIDB systems | Ship end-to-end natural-language database interfaces as production systems. | 1 |
| **Total** | | **33** |

---

## Trend Analysis

<div class="trend">
  <div class="plot">
    <div class="bcol">
      <div class="bcount">1</div>
      <div class="stack">
        <div class="seg bench" style="height:14px"></div>
      </div>
    </div>
    <div class="bcol">
      <div class="bcount">2</div>
      <div class="stack">
        <div class="seg schema" style="height:14px"></div>
        <div class="seg ind" style="height:14px"></div>
      </div>
    </div>
    <div class="bcol">
      <div class="bcount">1</div>
      <div class="stack">
        <div class="seg schema" style="height:14px"></div>
      </div>
    </div>
    <div class="bcol">
      <div class="bcount">5</div>
      <div class="stack">
        <div class="seg bench" style="height:14px"></div>
        <div class="seg schema" style="height:14px"></div>
        <div class="seg llm" style="height:14px"></div>
        <div class="seg rank" style="height:14px"></div>
        <div class="seg slm" style="height:14px"></div>
      </div>
    </div>
    <div class="bcol">
      <div class="bcount">13</div>
      <div class="stack">
        <div class="seg bench" style="height:14px"></div>
        <div class="seg schema" style="height:42px"></div>
        <div class="seg llm" style="height:42px"></div>
        <div class="seg agentic" style="height:28px"></div>
        <div class="seg rank" style="height:28px"></div>
        <div class="seg slm" style="height:28px"></div>
      </div>
    </div>
    <div class="bcol">
      <div class="bcount">11</div>
      <div class="stack">
        <div class="seg bench" style="height:14px"></div>
        <div class="seg llm" style="height:84px"></div>
        <div class="seg agentic" style="height:42px"></div>
        <div class="seg rank" style="height:14px"></div>
      </div>
    </div>
  </div>
  <div class="years">
    <span>2018</span><span>2020</span><span>2021</span><span>2023</span><span>2024</span><span>2026</span>
  </div>
  <div class="chart-legend">
    <span><i class="dot" style="background:#1565c0"></i>Benchmarks</span>
    <span><i class="dot" style="background:#2e7d32"></i>Schema linking</span>
    <span><i class="dot" style="background:#ef6c00"></i>LLM prompting</span>
    <span><i class="dot" style="background:#00838f"></i>Agentic</span>
    <span><i class="dot" style="background:#6a1b9a"></i>Generate-then-rank</span>
    <span><i class="dot" style="background:#c62828"></i>SLM–LLM</span>
    <span><i class="dot" style="background:#546e7a"></i>Industrial</span>
  </div>
</div>

<ul class="findings">
  <li><strong>2024 is the peak (13 papers):</strong> schema linking, LLM prompting, agentic pipelines, ranking, and SLM–LLM work all appear together.</li>
  <li><strong>Early work (2018–2021, 4 papers)</strong> is dominated by benchmarks and pre-LLM neural parsing, with one industrial system.</li>
  <li><strong>By 2026 the frontier shifts</strong> to LLM prompting/decomposition (6) and agentic multi-agent systems (3), while surveys consolidate the field.</li>
</ul>

<div class="sources">
<b>Sources:</b> counts derived from the 33-paper table in <code>src/main.tex</code>, grouped by publication year and research front.
</div>

---

## Schema Linking \& Neural Parsing

<div class="definition">
<strong>Schema linking</strong> grounds mentions in the question—entities, values, and implicit references—to schema elements: tables, columns, and the join paths between them. <strong>Neural parsing</strong> then turns the grounded question into SQL, either by learning the alignment inside an encoder–decoder or by consuming an explicitly linked schema.
</div>

| | Mechanism | Consequence |
|:--|:--|:--|
| **Pro** | Prune irrelevant tables and columns | Shorter prompts, smaller decoding space, lower inference cost |
| **Pro** | Match names, values, and foreign keys | Grounds predicates and JOINs; fewer hallucinated columns and values |
| **Pro** | Focus the parser on a compact schema | Higher accuracy on large, noisy, multi-table databases |
| **Risk** | Any missed element is unrecoverable | A missing table, column, or join path makes the SQL wrong by construction |
| **Risk** | Context can be removed with the noise | Even at high recall, simplified schemas may flip a correct query to incorrect (RSL-SQL's gain–loss trade-off) |
| **Risk** | Linking is brittle under distribution shift | Synonyms, perturbations, and unseen schemas break the linker; errors compound downstream |

<div class="takeaway">
<strong>Schema linking is a precision–recall bet, not a free preprocessing step.</strong> Pruning helps only when the linker keeps every element the SQL needs—and keeps enough context to disambiguate it.
</div>

<div class="sources">
<b>Sources:</b> RAT-SQL (2020) — name/value-based linking and schema generalization. RESDSQL (2023) — recall-versus-noise trade-off when filtering schema items. RSL-SQL (2024) — omission and structural-integrity risks; net benefit <code>y - x</code>. E-SQL (2024) — schema filtering can hurt strong LLMs. PICARD (2021) — schema-valid decoding as a complementary guard.
</div>

---

## How Schema Linking Works: A Worked Example

<div class="definition">
<strong>Question:</strong> “What are flight numbers of flights departing from City ‘Aberdeen’?”<br />
<strong>Schema:</strong> <code>airlines(uid, airline, abbreviation, country)</code>, <code>airports(city, airportcode, airportname, country, countryabbrev)</code>, <code>flights(airline, flightno, sourceairport, destairport)</code>
</div>

<div class="pipeline">
  <div class="step"><b>1 · Detect mentions</b>“flight numbers” → <code>flights.flightno</code>; “flights” → <code>flights</code>; “City” → <code>airports.city</code>; “Aberdeen” → a value of <code>airports.city</code>.</div>
  <div class="step"><b>2 · Link tables</b>“Aberdeen” can only be grounded through <code>airports</code>, so that table enters the linked set even though the question never says “airports”.</div>
  <div class="step"><b>3 · Recover the join</b>“departing from” has no lexical match; the linker must use the foreign key <code>flights.sourceairport → airports.airportcode</code>.</div>
  <div class="step"><b>4 · Filter and decode</b>Keep only <code>flights</code> and <code>airports</code>, rank their columns, and let the parser generate SQL.</div>
</div>

<div class="example">
  <div class="panel nl">
    <span class="label">Linked schema (RESDSQL-style)</span>
    <p><code>flights: airline, flightno, sourceairport, destairport</code><br /><code>airports: city, airportcode, airportname</code><br /><code>FK: flights.sourceairport = airports.airportcode</code></p>
  </div>
  <div class="arrow">→</div>
  <div class="panel sql">
    <span class="label">Executable SQL</span>
    <p><code>SELECT flights.flightno<br />FROM flights<br />JOIN airports<br />&nbsp;&nbsp;ON flights.sourceairport = airports.airportcode<br />WHERE airports.city = 'Aberdeen';</code></p>
  </div>
</div>

<div class="takeaway">
<strong>The hard part is not “Aberdeen”.</strong> Lexical matches are easy; the linker must also infer the unmentioned <code>airports</code> table and the <code>departing from</code> join—exactly the information that a purely name-based matcher misses.
</div>

<div class="sources">
<b>Sources:</b> RESDSQL (2023, Figure 1) — the Aberdeen flights example, schema serialization, filtering, and skeleton-aware decoding. RAT-SQL (2020, Figure 1) — the same ambiguity problem framed as name-based and value-based linking over a schema graph.
</div>

---

## Schema Linking - Three Insights

| Paper | Insight | Linking mechanism | What it optimizes |
|:--|:--|:--|:--|
| **RAT-SQL** (2020) | memory-schema alignment should be a first-class relation in the parser. | Typed relation-aware self-attention; explicit memory–schema alignment matrices. | End-to-end parser accuracy and interpretable alignment. |
| **RESDSQL** (2023) | Separate linking from skeleton parsing to decouple schema item and SQL keywords. | A cross-encoder ranks and filters tables/columns; the decoder emits the SQL skeleton first, then fills it. | Recall-versus-noise balance in preprocessing, plus structural guidance during decoding. |
| **E-SQL** (2024) | Enrich the question instead of pruning the schema to work with stronger LLMs. | Candidate SQL → candidate predicates → question enrichment with tables, columns, values, and a construction plan → refinement; no schema filtering. | Semantic alignment and reasoning, especially on complex predicates and small LLMs. |

<div class="takeaway">
<strong>Same goal, three loci of control:</strong> inside the encoder (RAT-SQL), before the encoder (RESDSQL), and in the question/prompt (E-SQL). None chooses a linking strategy adaptively per query—the linking policy is fixed in advance.
</div>

<div class="sources">
<b>Sources:</b> RAT-SQL (2020, ACL), Section 4.3 and Figure 1; RESDSQL (2023, AAAI), Sections 1 and 4; E-SQL (2024, arXiv:2409.16751), Sections 1 and 3.5. Companion results: RSL-SQL (2024) — bidirectional linking and the gain/loss analysis; Solid-SQL (2024) — robust schema-linking model with LLM-based data augmentation; PICARD (2021) — constrained decoding against invalid schema references.
</div>

---

## LLM Prompting \& Decomposition

<div class="definition">
<strong>LLM prompting / decomposition</strong> uses <strong>staged chain of prompts</strong>: ground the question in the schema, <strong>break the task into sub-tasks</strong>, generate candidate queries, then correct/select the best.
</div>

| | Mechanism | Consequence |
|:--|:--|:--|
| **Pro** | Decompose generation into linking, classification, generation, correction | Splits a hard declarative task into sub-problems the LLM solves more reliably (DIN-SQL: ~10% gain) |
| **Pro** | Few-shot prompting instead of fine-tuning | No task-specific data or heavy compute; decomposition also lifts small open models (DTS-SQL, LearNAT) |
| **Pro** | Multi-prompt sampling + self-correction / error modeling | Prompt sensitivity becomes diversity; selection and repair recover the best query (MCS-SQL, SelECT-SQL, ErrorLLM) |
| **Risk** | LLMs are sensitive to prompt wording and order | The same question yields different SQL; accuracy is brittle across prompts |
| **Risk** | Decomposing declarative SQL is ill-defined | Sub-task boundaries are unclear; an intermediate error propagates to the final query |
| **Risk** | Multi-round prompts cost tokens/latency; self-correction can hallucinate | Gains trade against inference budget; low detection precision can corrupt a correct SQL |

<div class="takeaway">
<strong>Decomposition pays off only if the split is right and the loop is closed.</strong> Otherwise prompt noise, propagation of intermediate errors, and self-correction hallucination erode the accuracy gains.
</div>

<div class="sources">
<b>Sources:</b> DIN-SQL (2023) — prompting avoids training data and fine-tuning; sub-task decomposition gains ~10%. DTS-SQL (2024) and LearNAT (2026) — privacy/cost of proprietary models and test-time scaling cost. MCS-SQL (2024) — prompt sensitivity exploited as diversity. SelECT-SQL (2024) — CoT + self-correction + ensemble and its token cost. ErrorLLM (2026) — self-debugging fails and self-correction hallucinates. Yuan et al. / KaSLA (2026) — missing or redundant schema elements propagate to SQL.
</div>

---

## The Decomposed Prompting Pipeline

<div class="definition">
The workflow converges on the same four stages: <strong>link → decompose → generate → correct/select</strong>. The papers differ in <em>task decomposition</em> and <em>aggregating/repairing candidates</em>.
</div>

<div class="pipeline">
  <div class="step"><b>1 · Schema link</b>Ground the question in relevant tables and columns.</div><!-- —via shuffled multi-prompts (MCS-SQL) or knapsack-optimal linking (KaSLA) -->
  <div class="step"><b>2 · Classify & decompose</b>Label difficulty and split into sub-tasks: easy/non-nested/nested, CoT, or AST-guided.</div><!-- (DIN-SQL) (SelECT-SQL) (LearNAT)-->
  <div class="step"><b>3 · Generate candidates</b>Emit SQL from class-specific prompts, producing candidate queries.</div>
  <div class="step"><b>4 · Correct & select</b>Self-correct, then filter and choose.</div>
</div>

<div class="example">
  <div class="panel nl">
    <span class="label">Decomposed sub-tasks</span>
    <p><code>1</code> link <code>employees.salary</code>, self-join on <code>manager</code><br /><code>2</code> classify: non-nested (join, no subquery)<br /><code>3</code> generate join + salary comparison<br /><code>4</code> correct join condition & predicate</p>
  </div>
  <div class="arrow">→</div>
  <div class="panel sql">
    <span class="label">Final SQL</span>
    <p><code>SELECT e.name FROM employees e<br />JOIN employees m ON e.manager_id = m.id<br />WHERE e.salary > m.salary;</code></p>
  </div>
</div>

<div class="takeaway">
<strong>The decisive choices are the split and the aggregator.</strong> Decomposition alone helps, but the state-of-the-art comes from combining a task-aware split with candidate selection or error-driven repair.
</div>

<div class="sources">
<b>Sources:</b> DIN-SQL (2023, Fig. 2) — schema linking → classification & decomposition → class-specific generation → self-correction. MCS-SQL (2024, Fig. 1) — schema linking → multiple generation → filtering → multiple-choice selection. SelECT-SQL (2024) — SS/MS CoT, self-correction, and ensemble. LearNAT (2026, Fig. 1) — AST-guided verifiable decomposition. ErrorLLM (2026) — static detection, error tokens, error-guided refinement. KaSLA (2026) — hierarchical table-then-column knapsack linking.
</div>

---

## LLM Prompting - Three Insights

| Paper | Insight | Mechanism |
|:--|:--|:--|
| **DIN-SQL** (2023) | Break the declarative SQL task into sub-problems and feed each sub-solution forward. | Four prompting modules—schema linking, difficulty classification & decomposition, class-specific generation, self-correction—all in-context, no fine-tuning. |
| **MCS-SQL** (2024) | Prompt sensitivity is a diversity source, not noise: sample widely, then aggregate. | Shuffled multi-prompts for linking and generation; confidence filtering by shared execution results; LLM multiple-choice selection. |
| **ErrorLLM** (2026) | Refinement fails because errors are never modeled; detect and name error types before fixing. | Static detection plus dedicated error tokens for implicit semantic errors; error-guided structural refinement via prompting. |

<div class="takeaway">
<strong>The front matures from "split the prompt" to "learn and model the failure modes."</strong> DIN-SQL (2023) established decomposition prompting; MCS-SQL and SelECT-SQL (2024) layered multi-prompt ensembles and self-correcting CoT; LearNAT (2026) learns verifiable AST decompositions for 7B models, ErrorLLM (2026) models errors explicitly, and Royer et al. (2026) retargets generation to dialect-agnostic query plans.
</div>

<div class="sources">
<b>Sources:</b> DIN-SQL (2023, NeurIPS), Sections 4.1–4.4 — decomposition modules and self-correction. MCS-SQL (2024, arXiv:2405.07467), Sections 3.1–3.3 — multi-prompt linking, generation, and selection. ErrorLLM (2026, KDD) — error modeling and error-guided refinement. Companion results: DTS-SQL (2024) — two-stage fine-tuning for small LLMs; SelECT-SQL (2024) — SS/MS CoT with ensemble; LearNAT (2026, ICLR) — AST-guided decomposition + margin-aware RL; Royer et al. (2026, EMNLP Findings) — query-plan target; KaSLA (2026, ICDE) — knapsack schema linking.
</div>

---

## Generate-then-Rank \& Self-Correction

<div class="definition">
<strong>Generate-then-rank</strong>: the model produces a <strong>set of candidate queries</strong>, then a ranker or selection model picks the best. <strong>Self-correction</strong> closes the loop by repairing the chosen query against the DB schema or execution result.
</div>

| | Mechanism | Consequence |
|:--|:--|:--|
| **Pro** | Sample many candidates instead of one auto-regressive output | Escapes sub-optimal "top-1" decoding; ranking can recover a globally-optimal query |
| **Pro** | Rank on global NL↔SQL semantic similarity | Sidesteps the local, left-to-right context bias of sequential decoding |
| **Pro** | Wrap existing backends with metadata + ranking | Model-agnostic; lifts Seq2seq and LLM baselines without retraining the generator |
| **Pro** | Repair the winner against schema, dialect, execution | Fixes hallucinated columns, values, and operator misuse; stabilizes output |

---

## Generate-then-Rank \& Self-Correction (Cont.)

| | Mechanism (Cont.) | Consequence (Cont.) |
|:--|:--|:--|
| **Risk** | N× generation plus ranking overhead | Multiplies inference calls, latency, and cost; forces an accuracy–budget trade-off |
| **Risk** | Diversity ≠ correctness | More candidates can still all be wrong; self-consistency is not always the optimal selector |
| **Risk** | Ranker is a second point of failure | A wrong rank can demote the one correct candidate produced upstream |
| **Risk** | Generation is bounded by samples/metadata/demonstrations | Unseen components or operator compositions outside the covered set stay untranslatable |

<div class="takeaway">
<strong>Generate-then-rank trades compute for correctness—but only if both ends are strong.</strong> A diverse generator and an accurate ranker are each necessary: broad coverage fails without good ranking, and good ranking is wasted on narrow, near-duplicate candidates.
</div>

<div class="sources">
<b>Sources:</b> MetaSQL (2024, ICDE) — auto-regressive decoding suffers from low output diversity and missing global context; metadata + two-stage ranking as a model-agnostic fix. XiYan-SQL (2026, TKDE) — increased candidate diversity alone does not guarantee correctness, and self-consistency does not always select the optimum. PURPLE (2024, ICDE) — execution match overestimates quality, hallucination repair, and the cost/accuracy trade-off. GAR (2023, ICDE) — translation is bounded by the coverage of sample queries; unseen components are not generated.
</div>

---

## The Generate-then-Rank Pipeline

<div class="definition">
Conventional four-stage workflow: <strong>control → generate → rank → repair</strong>. The papers differ mainly in <em>what</em> control signal is used and <em>how</em> candidates are ranked.
</div>

<div class="pipeline">
  <div class="step"><b>1 · Control / Understand</b>Map the NL meaning to a control signal — query metadata (MetaSQL), a predicted SQL skeleton (PURPLE), or generalized sample queries (GAR).</div>
  <div class="step"><b>2 · Generate candidates</b>Condition diverse decoders/generators on the control signal to emit many SQL candidates (metadata-conditioned, multi-generator, component-recomposed).</div>
  <div class="step"><b>3 · Rank / Select</b>Score NL↔SQL similarity globally with learning-to-rank or a selection model, then pick the best candidate.</div>
  <div class="step"><b>4 · Self-correct</b>Adapt the winner to the schema and DBMS dialect, and validate by execution; fix hallucinations and stabilize the output.</div>
</div>

<div class="example">
  <div class="panel nl">
    <span class="label">Candidates (diverse but uneven)</span>
    <p><code>… WHERE language != 'English'</code><br /><code>… JOIN Country WHERE …</code><br /><code>… EXCEPT SELECT … WHERE language='English'</code></p>
  </div>
  <div class="arrow">→</div>
  <div class="panel sql">
    <span class="label">Ranked output (MetaSQL)</span>
    <p><code>SELECT countrycode FROM CountryLanguage<br />EXCEPT SELECT countrycode FROM CountryLanguage<br />WHERE language='English';</code></p>
  </div>
</div>

<div class="takeaway">
<strong>The decisive step is ranking, not generation.</strong> For “countries that do not speak English”, beam-search top-1..5 are near-duplicate wrong answers; the ranker—using whole-query context—recovers the <code>EXCEPT</code> formulation the generator could produce but could not prioritize.
</div>

<div class="sources">
<b>Sources:</b> GAR (2023, ICDE), Fig. 2 — generalize → SQL2NL → learning-to-rank. MetaSQL (2024, ICDE), Fig. 1 & Fig. 2 — the CountryLanguage <code>EXCEPT</code> example and semantic-decomposition → metadata-conditioned generation → two-stage ranking. PURPLE (2024, ICDE), Fig. 3 — schema pruning → skeleton prediction → demonstration selection → LLM inference → database adaption. XiYan-SQL (2026, TKDE), Fig. 1 — schema filter → multiple SQL generation → SQL selection.
</div>

---

## Generate-then-Rank - Three Insights

| Paper | Insight | Mechanism |
|:--|:--|:--|
| **MetaSQL** (2024) | Single auto-regressive SQL is trapped in local optima and near-duplicate beams; rank over the whole query instead. | Query metadata as an explicit control signal; metadata-conditioned candidate generation; two-stage retrieve-then-rerank pipeline. |
| **PURPLE** (2024) | The bottleneck is logical operator composition, not NL understanding; retrieve demos that teach it, then repair the output. | Fine-tuned skeleton predictor → 4-level skeleton abstraction → demonstration retrieval; database-adaptation self-correction with execution-consistency. |
| **XiYan-SQL** (2026) | Diversity alone is insufficient; combine an ensemble of expert generators with a learned selector. | Multi-path schema filtering + multi-task / multi-format fine-tuned generators + selection model with candidate reorganization. |

<div class="takeaway">
<strong>The front matures from rank to repair.</strong> GAR (2023) originated the idea—generalize sample SQL, render it as dialect text, and rank by semantic match—but stays within the covered query space. MetaSQL makes generation controllable, PURPLE adds skeleton-guided demonstration retrieval and self-correction, and XiYan-SQL scales to a fine-tuned multi-generator ensemble with a learned selector.
</div>

<div class="sources">
<b>Sources:</b> MetaSQL (2024, ICDE), Sections 1 and 3 — metadata design, metadata-conditioned generation, two-stage ranking. PURPLE (2024, ICDE), Sections 1 and 3–4 — logical-operator-composition motivation, skeleton prediction, demonstration selection, database adaption. XiYan-SQL (2026, TKDE), Sections 1 and 3 — hybrid ensemble philosophy, multi-task/multi-format fine-tuning, candidate reorganization + selection model. GAR (2023, ICDE), Sections 1–3 — compositional generalization, SQL2NL dialect expressions, learning-to-rank.
</div>
