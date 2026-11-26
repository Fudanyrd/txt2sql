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

<!-- FIXME: -->
<div class="title">
Counterexample-Guided Formal Verification for Agentic Text-to-SQL Refinement
</div>

<div class="kicker">A Research Proposal</div>

<div class="author">
Rundong Yang, Jindi Yao, Yanwen Sun, Han Han, Yutong Chen, and Zhaohan Chu
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
<strong>Decomposed prompting</strong> gives the LLM a series of smaller tasks, from identifying the relevant schema to checking the generated SQL.
</div>

| | Mechanism | Consequence |
|:--|:--|:--|
| **Pro** | Break the task into smaller steps | The model can identify the schema and plan the query before writing SQL. |
| **Pro** | Give examples in the prompt (DIN-SQL) | The model uses those examples without task-specific fine-tuning. |
| **Pro** | Try multiple prompt variations | Different prompts can produce different SQL candidates to choose from. |
| **Risk** | Change wording or example order | Even small prompt changes can affect accuracy. |
| **Risk** | Carry intermediate results forward | An early mistake, such as choosing the wrong join key, can reach the final SQL. |
| **Risk** | Add generation or repair rounds | More calls use more tokens and take longer. Repair can introduce errors. |

<div class="takeaway">
<strong>DIN-SQL with GPT-4 on the Spider development set</strong><br />Execution accuracy rose from <strong>67.4% to 74.2%</strong> compared with simple few-shot prompting.
</div>

<div class="sources">
<b>Sources:</b> DIN-SQL (2023, Table 4a), MCS-SQL (2024), SelECT-SQL (2024), ErrorLLM (2026). DTS-SQL (2024) and LearNAT (2026) study decomposition with training.
</div>

---

## The Decomposed Prompting Pipeline

<div class="definition">
<strong>Question</strong> What are the names of employees who earn more than their direct managers?<br />
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
    <p style="font-size: 16px; line-height: 1.3;">
      <strong>1. Link</strong> Name → <code>name</code>, pay → <code>salary</code>, manager → <code>manager_id</code>.<br />
      <strong>2. Classify &amp; decompose</strong> Non-nested. Match each employee to their manager, then compare pay.<br />
      <strong>3. Generate</strong> Write the plan in SQL with <code>JOIN</code>, <code>WHERE</code>, and <code>SELECT</code>.<br />
      <strong>4. Correct</strong> Check the manager match and strict <code>&gt;</code> against the question.
    </p>
  </div>
  <div class="arrow">→</div>
  <div class="panel sql">
    <span class="label">Final SQL</span>
    <pre style="margin: 0; padding: 0; border: 0; background: transparent;"><code>SELECT e.name
FROM employees AS e
JOIN employees AS m
  ON e.manager_id = m.id
WHERE e.salary &gt; m.salary;</code></pre>
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

---

## Agentic LLM (Multi-Agent)

<div class="definition">
<strong>Agentic Text-to-SQL</strong> replaces the single model with a set of <strong>specialized LLM agents</strong>—for schema retrieval, decomposition, generation, execution, and repair.
<!-- —that coordinate through a shared loop of <strong>plan → act → observe → revise</strong> -->
</div>

| | Mechanism | Consequence |
|:--|:--|:--|
| **Pro** | Split the task across specialist agents | Each agent owns one sub-problem (retrieval, generation, refinement), so the pipeline handles huge schemas and multi-step questions a monolithic prompt cannot (MAC-SQL) |
| **Pro** | Close the loop with tools and execution feedback | Agents execute SQL and inspect real data, so errors are caught and corrected instead of guessed (MAC-SQL, APEX-SQL) |
| **Pro** | Prune context on demand and decouple the model | A schema-selector agent cuts large catalogs to a sub-schema (~2% gain, ~5× fewer tokens); roles also run on a 7B open model for cost/privacy (CHESS, MAC-SQL) |
| **Risk** | Many agents mean many LLM calls | Multi-round coordination multiplies latency and token cost; accuracy is bought with compute budget (CHESS) |
| **Risk** | A single bad handoff poisons the result | A wrong retrieval, a dropped ambiguity, or a premature "done" propagates into a wrong final SQL (PLANPOOL) |
| **Risk** | Coordination state is itself a new failure mode | Agents forget planned steps, retrieve irrelevant memory, or halt clarification early—correct execution can still mask unresolved intent (PLANPOOL, MERIT) |

<div class="takeaway">
<strong>Multi-agent decomposition helps only if every handoff and every "done" is guarded.</strong> The gains come from specialization and execution feedback; the costs are multiplied calls, error propagation, and a new class of coordination failures.
</div>

<div class="sources">
<b>Sources:</b> MAC-SQL (2024) — degradation on huge databases and complex multi-step questions; external tools and model collaboration; Selector/Decomposer/Refiner roles and the SQL-Llama cost trade-off. CHESS (2024) — schema-selector token/accuracy trade-off and open-source privacy-preserving deployment. APEX-SQL (2026) — static-schema guessing vs. grounding in real data. MERIT (2026) — static and single-horizon memory mismatch. PLANPOOL (2026) — premature clarification termination and silent, unverified assumptions.
</div>

---

## The Multi-Agent Text-to-SQL Workflow

<div class="definition">
Same <strong>agentic loop</strong>: <strong>retrieve & prune → generate → execute/verify → refine</strong> is adopted. They differ in <em>agents&apos; role</em> and <em>loop termination</em>—execution results, unit tests, data profiling, or user clarification.
</div>

<div class="pipeline">
  <div class="step"><b>1 · Retrieve & prune</b>A Schema Selector + Information Retriever grounds the question and prunes the schema and values.</div>
  <div class="step"><b>2 · Decompose & generate</b>A Decomposer splits complex questions into sub-questions; a generator emits candidate SQL.</div><!-- (MAC-SQL, CHESS)-->
  <div class="step"><b>3 · Execute & verify</b>A Refiner inspects errors, a Unit Tester checks NL unit tests, or profiles real data.</div><!--  (MAC-SQL, CHESS, APEX-SQL)-->
  <div class="step"><b>4 · Refine & iterate</b>Feedback drives revision—rewrite the SQL, re-ask the user, or re-explore.</div>
</div>

<div class="example">
  <div class="panel nl">
    <span class="label">Agent trace (MAC-SQL)</span>
    <p><code>Selector</code> → keep <code>frpm</code>, <code>satscores</code>, <code>schools</code><br />
    <code>Decomposer</code> → sub-Q1: average SAT rate; sub-Q2: names above it<br />
    <code>Refiner</code> → SQL error on <code>Charter School (Y/N)</code> → fix predicate</p>
  </div>
  <div class="arrow">→</div>
  <div class="panel sql">
    <span class="label">Final SQL</span>
    <p><code>SELECT sname FROM frpm JOIN satscores<br />ON CDSCode = cds<br />WHERE Charter = 1 AND rate > (SELECT AVG(...) ...);</code></p>
  </div>
</div>

<div class="takeaway">
<strong>The loop is shared; the differentiator is the feedback signal.</strong> Execution errors (MAC-SQL), LLM unit tests (CHESS), data profiling (APEX-SQL), and user clarification (PLANPOOL) each close the loop against a different kind of ground truth.
</div>

<div class="sources">
<b>Sources:</b> MAC-SQL (2024, Fig. 2) — Selector → Decomposer → Refiner with SQL-execution feedback. CHESS (2024, Fig. 2) — IR/SS/CG/UT agent pipeline. APEX-SQL (2026, Fig. 1c) — hypothesis-verification loop over real data. PLANPOOL (2026) — clarification as part of the interactive loop.
</div>

---

## Agentic LLM - Three Insights

| Paper | Insight | Mechanism |
|:--|:--|:--|
| **MAC-SQL** (2024) | A monolithic prompt degrades on huge schemas and multi-step questions; break the task across collaborating specialist agents. | Three agents—Selector (sub-database), Decomposer (sub-questions + CoT), Refiner (execution feedback)—activated as needed. |
| **APEX-SQL** (2026) | Static schemas make the model guess; shift from passive translation to agentic exploration grounded in real data. | Hypothesis-verification loop: logical planning, dual-pathway pruning, parallel data profiling, global synthesis; deterministic retrieval of exploration directives during generation. |
| **PLANPOOL** (2026) | Correct execution ≠ resolved intent: agents silently drop ambiguities they already identified. | Externalize the clarification plan as a mutable question pool; every planned question must be asked or explicitly dropped before the SQL is submitted. |

<div class="takeaway">
<strong>The front matures from "who does what" to "what grounds the answer."</strong> MAC-SQL (2024) established agent collaboration; CHESS (2024) made it cost-efficient and privacy-preserving; APEX-SQL (2026) grounds it in data, MERIT (2026) in learned memory, and PLANPOOL (2026) in the user's actual intent.
</div>

<div class="sources">
<b>Sources:</b> MAC-SQL (2024, NAACL), Sections 1 and 3 — agent roles, tools, and SQL-Llama. APEX-SQL (2026, KDD), Sections 1 and 3 — hypothesis-verification and exploration directives. PLANPOOL (2026, arXiv:2610.02739), Sections 1 and 4 — premature clarification termination and the question-pool mechanism. Companion results: CHESS (2024) — IR/SS/CG/UT with unit-test verification; MERIT (2026, EMNLP) — dual-level memory retrieval with RL.
</div>

---

## Text-to-SQL Dataset \& Benchmark

| Paper | \# Questions | Data Source | Evaluation Metric |
|:--|:--|:--|:--|
| **Spider** (2018) | 10,181 | 200 databases, 138 domains (human-labeled) | Exact-set match (EM) accuracy |
| **BIRD** (2023) | 12,751 | 95 databases (33.4 GB), 37 domains | Execution accuracy (EX) + efficiency (VES) |
| **Spider 2.0** (2024) | 632 | Enterprise databases (BigQuery, Snowflake; >1,000 cols) | Task success rate (execution-based) |
| **SpotIt** (2026) | N/A | Reuses BIRD (10 methods) | Formal bounded equivalence verification |
||||

---

<h1>Our Research Proposal</h1>

---

## Introduction

<div class="definition">
<strong>Agentic Text-to-SQL</strong> loops <strong>retrieval → candidate generation → verification → refinement</strong>. Its weakest link is <strong>when to stop</strong>: prior systems terminate on <em>execution success</em> (MAC-SQL) or <em>LLM-generated unit tests</em> (CHESS) — signals that are <strong>necessary but not sufficient</strong> to guarantee a correct query.
</div>

<br/>
<div class="takeaway">
<strong>The gap:</strong> formal verification is used only <em>offline</em> — SpotIt checks bounded equivalence against a <em>gold query</em>. <strong>No prior method uses it to guide refinement online</strong>, where no gold query exists.
</div>

<br/>
<div class="definition">
<strong>Our approach:</strong> a <strong>Critic Agent</strong> states the correctness criteria given the question and schema; a <strong>bounded SMT verifier</strong> searches for a <em>counterexample database</em> that differentiates the candidate from those criteria, and returns it as <strong>concrete repair evidence</strong>. <strong>Verification — not execution success — terminates the loop.</strong>
</div>

<div class="sources">
<b>Sources:</b> MAC-SQL (2024) — execution-success termination. CHESS (2024) — LLM unit-test termination. SpotIt (2026) — offline bounded-equivalence verification against a gold query. ErrorLLM (2026) — heuristic error detection. BIRD (2023) — evaluation benchmark.
</div>

---

## Contributions

<div class="card-grid">
  <div class="card">
    <span class="badge">C1</span>
    <h3>Verification-guided refinement</h3>
    <p>First method to steer agentic refinement with a bounded SMT verifier <strong>online</strong>, yielding a <strong>sound differentiating witness</strong> instead of heuristic error detection (ErrorLLM).</p>
  </div>
  <div class="card">
    <span class="badge teal">C2</span>
    <h3>Tractable criteria synthesis</h3>
    <p>Synthesize <strong>verifiable correctness criteria</strong> from question + schema — distinct from full SQL generation — to close the <strong>specification gap</strong>.</p>
  </div>
  <div class="card">
    <span class="badge green">C3</span>
    <h3>Counterexample-guided repair</h3>
    <p>Return counterexamples as concrete repair evidence and terminate on verification; evaluated on <strong>BIRD</strong> to close the <strong>silent-error gap</strong>.</p>
  </div>
</div>

---

## Research Questions

<div class="card-grid">

<div class="card">
<span class="badge">RQ1</span>
<h3>Effectiveness</h3>
<p>Does counterexample-guided verification improve end-to-end accuracy over agentic baselines that terminate on execution success or LLM unit tests?</p>
</div>

<div class="card">
<span class="badge teal">RQ2</span>
<h3>Silent errors</h3>
<p>Does verification close the <strong>silent-error gap</strong> — queries that execute correctly on the test database yet are not equivalent to the gold query — that execution-based evaluation overlooks?</p>
</div>

<div class="card">
<span class="badge green">RQ3</span>
<h3>Ablation</h3>
<p>What does each component — criteria synthesis, counterexample-guided repair, verification-based termination — contribute to the overall gain?</p>
</div>

</div>

<div class="takeaway">
<strong>Three questions, one target:</strong> show that formal verification moves the needle on accuracy, isolates the failure mode execution-based metrics miss, and attributes the gain to each part of the loop.
</div>

<div class="sources">
<b>Sources:</b> <code>src/proposal.tex</code>, "Experiments" — RQ1 (effectiveness), RQ2 (silent errors), RQ3 (ablation).
</div>

---

## Experimental Setup

<div class="definition">
<strong>Dataset.</strong> <strong>BIRD</strong> — 12,751 question–SQL pairs over 95 databases spanning 37 domains (33.4 GB), each with external knowledge and a reference answer. We tune and ablate on the <strong>development set (1,534 examples)</strong> and report final numbers on the held-out <strong>test set</strong>. BIRD's large, noisy, multi-table schemas stress exactly the retrieval and refinement stages where execution-feedback agents most often fail.
</div>

| Metric | Definition | Why it matters |
|:--|:--|:--|
| **EX** | Execution accuracy — predictions whose execution matches the gold result | BIRD's primary score |
| **VES** | Valid efficiency score — EX discounted for correct-but-inefficient queries | Captures efficiency, not just correctness |
| **SER** | Silent-error rate — execute correctly but not boundedly equivalent to gold (via SpotIt) | Isolates the failure mode our verifier targets |

<div class="chips">
  <div class="chip">DIN-SQL — non-agentic single-pass frontier</div>
  <div class="chip">MAC-SQL — terminates on execution success</div>
  <div class="chip">CHESS — terminates on LLM unit tests</div>
  <div class="chip">Same backbone LLM across baselines</div>
</div>

<div class="takeaway">
<strong>Baselines span both termination signals we replace</strong> (execution success, LLM unit tests). Two self-ablations isolate our additions: (a) replace the SMT verifier with execution-success termination, and (b) remove counterexample-guided repair, leaving only criteria synthesis.
</div>

<div class="sources">
<b>Sources:</b> BIRD (Li et al., 2023) — dataset and EX/VES. SpotIt (Klopfenstein et al., 2026) — bounded-equivalence checker for SER. DIN-SQL (Pourreza & Rafiei, 2023), MAC-SQL (Wang et al., 2024), CHESS (Talaei et al., 2024) — baselines. PURPLE (Ren et al., 2024) — execution accuracy overestimates quality.
</div>

---

<h1>The End</h2>

<!-- 

## FAQ 

1. The methodology of your Research Proposal is missing.

Answer: Good catch! We are still working on it with crucial designs remain
to be determined.

2. Any publicly available artifacts (e.g. your paper list)?

Answer: these can be found at <a href="https://github.com/Fudanyrd/txt2sq>Github: Fudanyrd/txt2sql</a>.

3. Your Literature Review involves only 33 papers -- too few to support you
   trend analysis findings.

Answer: You are absolutely right in that regard -- our findings may be biased. However,
we tried our best to find (and keep) **most relevant** papers, far beyond the course
provided seeds.

4. You do not explain the scheme "SLM–LLM collaboration & open-source" at all.

Answer: We apologize for this negligence. However, we assume this can be justified by
limited presentation time (~20 minutes) and its low relevance to our research proposal.

x. Your work has a strong AI flavor.

Answer: While literature review is done by AI, searching relevant papers and forming the idea of
research proposal are done ourselves. Also, literature review is guided by a human-written skill
(therefore each part of them has similar structure).

-->
